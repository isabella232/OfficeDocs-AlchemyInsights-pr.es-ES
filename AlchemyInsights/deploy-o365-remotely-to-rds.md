---
title: Implementación de aplicaciones de Microsoft 365 para empresas para uso compartido en RDS, Terminal Server o VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200690"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementación de aplicaciones de Microsoft 365 para empresas para uso compartido en RDS, Terminal Server o VDI

Para implementar Aplicaciones de Microsoft 365 para empresas con Servicios de Escritorio remoto (RDS), anteriormente denominado Terminal Services:

- Debe tener un plan de Microsoft 365 Para empresas o un plan de Office 365 que incluya Aplicaciones de Microsoft 365 para empresas, como Office 365 Enterprise E3 o Enterprise E5.
   > [!NOTE]
   > Los planes Aplicaciones de Microsoft 365 para empresas y Microsoft 365 Empresa Standard no incluyen Aplicaciones de Microsoft 365 para empresas.
- Debe habilitar la [activación del equipo compartido](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> También puede descargar y ejecutar el Asistente para soporte técnico y recuperación de [Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) para instalar Aplicaciones de Microsoft 365 para empresas en modo de activación de equipos compartidos.

Para obtener más información sobre los requisitos previos, las instrucciones de configuración y las instrucciones sobre instalaciones personalizadas mediante la herramienta de implementación de Office, vea [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Para corregir errores relacionados con la activación de equipos compartidos:

- Consulte [Solucionar problemas con la activación de equipos compartidos para Aplicaciones de Microsoft 365 para empresas.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Vea [Restablecer el estado de activación de las aplicaciones de Microsoft 365 para empresas](https://go.microsoft.com/fwlink/?linkid=2109218).

Si desea instalar Aplicaciones de Microsoft 365 para empresas en RDS desde el Centro de administración de Microsoft 365, que usa la configuración de instalación predeterminada, siga estos pasos:

1. Comprueba qué suscripción tienes. [Obtenga más información](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Si es necesario, cambie a una suscripción diferente. [Obtenga más información](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Si Office ya está instalado en el servidor RDS con cualquier otra suscripción de Microsoft, desinstale. Por ejemplo, yendo al **Panel de control** Desinstalar un  >  **programa**. Desinstala con [el Asistente para soporte técnico y](https://aka.ms/SARA-OfficeUninstall-Alchemy) recuperación de Microsoft si tienes problemas.
4. En el servidor RDS, inicie sesión en el Centro de administración de Microsoft 365 con su cuenta de administrador e instale Aplicaciones de [Microsoft 365 para empresas.](https://portal.office.com/OLS/MySoftware.aspx)
5. Después de instalar Office, ***no abra ni inicie sesión en*** ninguna aplicación de Office.
6. En el servidor RDS, habilite la activación del equipo compartido editando el Registro siguiendo estos pasos:
   1. Haz clic con el botón derecho en el botón De Windows en la esquina inferior izquierda de la pantalla y selecciona **Ejecutar**. En el cuadro Abrir, escriba **regedit** y, luego, seleccione **Aceptar**.
   2. Seleccione **Sí** cuando se le pida que permita al Editor del Registro realizar cambios en el dispositivo.
   3. En el Editor del Registro, agregue un valor de cadena **de SharedComputerLicensing** con una configuración de 1 en HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. En el servidor RDS, ***inicie sesión*** como usuario final y compruebe que la activación del equipo compartido está habilitada para Aplicaciones de [Microsoft 365 para empresas.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
