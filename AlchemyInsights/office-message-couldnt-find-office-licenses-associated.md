---
title: 'Mensaje de aplicaciones de Microsoft 365: No ha sido posible encontrar las licencias de Office asociadas'
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
- "9001426"
- "3421"
ms.openlocfilehash: 16cc9d8d2ede108ea8301f9971f84ac7b6bafaabab8e26edefe15acf66783339
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54064971"
---
# <a name="microsoft-365-apps-message---couldnt-find-office-licenses-associated"></a>Mensaje de aplicaciones de Microsoft 365: No ha sido posible encontrar las licencias de Office asociadas

Para corregir este error, siga estos pasos:

- Elimine y [reasigne la licencia de Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) al usuario afectado.

- Abra una aplicación de Office y [cierre sesión](https://support.office.com/article/sign-out-of-office-5a20dc11-47e9-4b6f-945d-478cb6d92071) en las cuentas de usuario existentes.

- Vaya a **Configuración de Windows > Cuentas > Correo y cuentas** y elimine las cuentas de trabajo existentes.

- Vaya a **Configuración de Windows > Cuentas > Acceso profesional o educativo** y desconecte las cuentas existentes.

- Haga clic en el icono **+** para agregar o conectar su cuenta. Escriba las credenciales y espere a que se complete el proceso.

- Abra la aplicación de Office y, si es necesario, inicie sesión de nuevo.

Si el problema persiste, pruebe los siguientes pasos:

- Restablecer el estado de activación de Office. Consulte [Restablecer el estado de activación de las Aplicaciones de Microsoft 365 para empresas](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).

- Compruebe el firewall, el software antivirus y la configuración de proxy para confirmar que no están bloqueando el acceso de las aplicaciones de Microsoft 365 a Internet. 

Para ver más medidas de solución de problemas, vea:

[Errores de activación y de producto sin licencia en Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)

[Intervalos de direcciones IP y URL de Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
