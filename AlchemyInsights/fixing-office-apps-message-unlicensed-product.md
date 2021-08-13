---
title: No se ha podido activar Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928386"
---
# <a name="unable-to-activate-office"></a>No se ha podido activar Office

**Nota**: Si usa una versión anterior de Windows (por ejemplo, Windows 7), asegúrese de que TLS 1.2 esté habilitado como predeterminado. Para obtener más información, consulte [Actualizar para habilitar TLS 1.1 y TLS 1.2 como protocolos seguros predeterminados en WinHTTP en Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Compruebe el estado de la suscripción para ver si ha caducado.
- Asegúrese de que tiene una suscripción que permita licencias de cliente, así como Office 365 Empresa o Empresa Premium, y [asegúrese de que el usuario tenga asignada una licencia](/microsoft-365/admin/manage/assign-licenses-to-users).
- Asegúrese de que el usuario inicia sesión en Office con la misma cuenta a la que se ha asignado la licencia.
- Consulte la [página de estado del servicio de Office 365](/office365/enterprise/view-service-health) para ver si hay problemas conocidos con el servicio.
- Compruebe el firewall, el software antivirus y la configuración de proxy para confirmar que no bloquean el acceso de las aplicaciones de Microsoft 365 a Internet. Consulte [Intervalos de direcciones IP y URL de Office 365](/office365/enterprise/urls-and-ip-address-ranges "Intervalos de direcciones IP y direcciones URL de Office 365").

**Sugerencia** en equipos Windows, podemos diagnosticar y solucionar varios problemas comunes de inicio de sesión de Office. Descargue y ejecute el **[Asistente de soporte y recuperación de Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** para usar nuestra herramienta automatizada.

Haga lo siguiente para intentar solucionar el problema:

- Abra una aplicación de Office y [cierre sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) en las cuentas de usuario existentes. [Elimine](/microsoft-365/admin/manage/remove-licenses-from-users) y [reasigne](/microsoft-365/admin/manage/assign-licenses-to-users) la licencia de Office y, después, [inicie sesión en Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.
- Ejecute el [Solucionador de problemas de activación](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Restablezca el estado de activación de Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Restablezca el estado de activación de Office")
- [Realice una reparación en línea de Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Para ver más medidas de solución de problemas, vea:  

- [Errores de activación y de producto sin licencia en Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Error "Lo sentimos, no podemos conectarnos con su cuenta. Inténtelo de nuevo más tarde" al activar Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)