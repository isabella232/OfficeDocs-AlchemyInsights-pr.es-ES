---
title: Implementación de Aplicaciones Microsoft 365 para empresas para uso compartido en RDS, Terminal Server o VDI
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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041023"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementación de Aplicaciones Microsoft 365 para empresas para uso compartido en RDS, Terminal Server o VDI

Para implementar Aplicaciones Microsoft 365 servicios de Escritorio remoto (RDS), anteriormente Terminal Services, debe:

- Use la corrección fácil para habilitar TLS 1.2 de forma predeterminada si está ejecutando una versión anterior de Windows (por ejemplo, Windows 7 SP1, Windows Server 2008 R2). Para obtener una solución sencilla y más información, vea [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy). 
- Tener un plan que incluya Aplicaciones Microsoft 365 para empresas (anteriormente Office 365 Plus). Por ejemplo, Office 365 E3 o Microsoft 365 E5, o cualquier plan que incluya la versión de escritorio de Project o Visio, como Project Plan 3 o Visio Plan 2, o el plan Microsoft 365 Empresa Premium, que también incluye Aplicaciones Microsoft 365 para negocios.
- Habilitar la activación de equipos compartidos. Para obtener más información, vea [Overview of shared computer activation for Aplicaciones Microsoft 365](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Nota:** Para instalar Aplicaciones Microsoft 365 en modo de activación de equipo compartido, descargue y ejecute el archivo [de Microsoft Asistente de soporte y recuperación](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds). Para obtener información detallada sobre los requisitos previos, las instrucciones de configuración y las instrucciones para personalizar las instalaciones mediante la herramienta de implementación de Office, vea [Deploy Aplicaciones Microsoft 365 by using Remote Desktop Services](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Para corregir errores relacionados con la activación de equipos compartidos, vea:

- [Solucionar problemas con la activación de equipos compartidos para Aplicaciones Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Restablecimiento de las aplicaciones de Microsoft 365 para el estado de activación para empresas](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Si desea instalar Aplicaciones Microsoft 365 en RDS desde el Centro de administración de Microsoft 365, que usa la configuración de instalación predeterminada, siga estos pasos:

1. Compruebe qué Microsoft 365 plan tiene. Para obtener más información, vea [¿Qué suscripción tengo?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Si es necesario, cambie a un plan Microsoft 365 diferente. Para obtener más información, vea [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Si Aplicaciones Microsoft 365 ya está instalado en el servidor RDS con otros planes incompatibles, desinstale el programa yendo al **Panel de control** Desinstalar un  >  **programa**. Si tiene problemas, desinstale descargando [Microsoft Asistente de soporte y recuperación](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. En el servidor RDS, inicie sesión en el Centro de administración de Microsoft 365 con su cuenta de administrador e [instale Office](https://portal.office.com/OLS/MySoftware.aspx).

   Después Office instalado, no abra ni inicie sesión en ninguna Office aplicaciones.

1. En el servidor RDS, habilite la activación del equipo compartido editando el Registro:

   1. Haga clic con el botón Windows en la esquina inferior izquierda de la pantalla y seleccione **Ejecutar**. En el cuadro Abrir, escriba **regedit** y, luego, seleccione **Aceptar**.

   1. Cuando se le pida que permita al Editor del Registro realizar cambios en el dispositivo, seleccione **Sí**.

   1. En el Editor del Registro, en HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, agregue un valor de cadena **de SharedComputerLicensing** con una configuración de **1** .

1. En el servidor RDS, inicie sesión como usuario final y compruebe que la activación del equipo compartido está habilitada para Aplicaciones Microsoft 365. 

   Para obtener más información, vea [Verify that shared computer activation is enabled for Aplicaciones Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).