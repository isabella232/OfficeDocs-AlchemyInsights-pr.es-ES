---
title: El Acceso condicional con dispositivo unido a dominio me bloquea
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: d71bb376615191f507d39b99d9e51ca77d929b90
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323455"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>El Acceso condicional con dispositivo unido a dominio me bloquea

**Herramientas altamente recomendadas**

[Herramienta solucionador de problemas de registro de dispositivo](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/): la herramienta que ayuda a solucionar los problemas de registro de dispositivos más comunes.

[Script de conectividad de registro de dispositivos de prueba](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : el script que ayuda a asegurarse de que un dispositivo pueda tener acceso a los puntos de conexión de Registro de dispositivos en la cuenta del sistema.

[Script de limpieza de dispositivos de Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) : el script que le permite buscar y administrar dispositivos obsoletos en su entorno.

Aquí tiene algunos motivos habituales por los que el acceso condicional puede fallar en un dispositivo que se haya unido a un dominio (Azure AD híbrido).

1. **No hay PRT de Azure AD en el dispositivo**: debe asegurarse de que el dispositivo tenga el Token de Actualización Principal (PRT) de Azure AD. Para obtener más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Para comprobar que tiene PRT de Azure AD, puede ejecutar `dsregcmd/status` comando en el dispositivo y comprobar si “AzureAdPrt” es igual a “SÍ”.

Si “AzureAdPrt” es igual a “NO”, compruebe lo siguiente:

- **Si tiene un entorno federado con AD FS y las redes domésticas de los usuarios no lo pueden alcanzar**: en este caso, asegúrese de que sus puntos de conexión "usernamemixed" sean accesibles desde la extranet. Si su AD FS se encuentra detrás de una VPN, asegúrese de que los usuarios se conecten a la VPN y vuelvan a iniciar sesión en el dispositivo. Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Si el TPM del dispositivo es defectuoso y por tanto no puede autenticar el dispositivo**: compruebe "tpm.msc" para ver si el estado del TPM es "Listo". Si no es así, ejecute `dsregcmd/leave` y deje que el dispositivo se vuelva a unir a Azure AD. A continuación, inténtelo de nuevo. Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Está usando un proveedor de identidad de terceros que no admite el protocolo WS-Trust**. Como describimos en nuestros documentos, los dispositivos unidos a Azure AD híbrido no pueden funcionar en este caso. Contacte con su proveedor de identidad para obtener soporte técnico.

2. **Los usuarios usan el explorador Chrome sin las cuentas de Windows 10** o **extensiones de Office de Chrome no usan automáticamente el PRT en dispositivos unidos a AAD o a AAD híbrido**: esto provoca que cualquier directiva de acceso condicional basado en dispositivos falle, y en dicho caso se muestra el mensaje de error “Dispositivo no registrado”. Para usar el explorador Chrome correctamente, debe instalar “Cuentas de Windows 10” o "Extensión de Office para el explorador Chrome de los usuarios" mediante SCCM o Intune. Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Si no es posible instalar la extensión de forma remota, notifique a los usuarios para que instalen manualmente una de las extensiones anteriores para acceder a aplicaciones detrás del acceso condicional basado en dispositivos. Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **El dispositivo estaba unido a Azure AD híbrido correctamente, pero se eliminó o se deshabilitó de manera accidental, ya sea debido a cambios en la sincronización en Azure AD Connect o desde Azure Portal**: si esto sucede, el objeto de dispositivo ya no será reconocido como dispositivo unido de manera completa, aunque los estados "AzureAdJoined" y "PRT" se muestren como válidos en el dispositivo.

Para solucionar este problema, ejecute `dsregcmd/leave` en los dispositivos afectados y deje que se vuelvan a unir a Azure AD. Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

**Nota**: Si sus dispositivos usan Windows 10, actualización 1809, con VPN/Cloud proxy y observa problemas con el estado "AzureAdPrt" o cualquier aplicación con problema de SSO (Outlook no se conecta al buzón de correo pese a tener PRT), asegúrese de tener esta revisión [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) o la actualización acumulativa de abril [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) para prevenir errores de PRT en esos equipos.

















