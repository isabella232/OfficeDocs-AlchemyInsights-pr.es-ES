---
title: 'Instalación de office en un Terminal Server: sin licencia'
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055175"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalación Office en un Terminal Server

Para implementar Aplicaciones Microsoft 365 para empresas en un servidor Windows mediante Servicios de Escritorio remoto (RDS), anteriormente denominado Terminal Services:
  
- Debe tener una suscripción Microsoft 365 que incluya Aplicaciones Microsoft 365 para empresas, como Office 365 Enterprise E3 o Enterprise E5. Los Aplicaciones Microsoft 365 para negocios y Aplicaciones Microsoft 365 para negocios Premium no incluyen Aplicaciones Microsoft 365 para empresas.

- Debe habilitar la activación [del equipo compartido.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Si desea instalar Aplicaciones Microsoft 365 para empresas en RDS desde el Centro de administración de Microsoft 365, que usa la ***configuración de*** instalación predeterminada, siga estos pasos.

> [!TIP]
> También puede descargar y ejecutar microsoft Asistente de soporte y recuperación [para](https://aka.ms/SaRA_OfficeSCA_M365Portal) instalar Aplicaciones Microsoft 365 para empresas en modo de activación de equipo compartido.
  
1. Comprueba qué Microsoft 365 suscripción tienes. [Más información](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Si es necesario, cambie a una suscripción Microsoft 365 diferente. [Más información](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Si Office ya está instalado en el servidor RDS con cualquier otra Microsoft 365 suscripciones, desinstale. Por ejemplo, yendo al Panel de control \> Desinstalar un programa. [Desinstale con Microsoft Asistente de soporte y recuperación](https://aka.ms/SARA-OfficeUninstall-Alchemy) si tiene problemas.

4. En el servidor RDS, inicie sesión en el Centro de administración de Microsoft 365 con su cuenta de administrador e [instale Aplicaciones Microsoft 365 para empresas](https://portal.office.com/OLS/MySoftware.aspx).

5. Después Office instalado, no ***abra*** ni inicie sesión en ninguna Office aplicaciones.

6. En el servidor RDS, habilite la activación del equipo compartido editando el Registro siguiendo estos pasos:

1. Haga clic con el botón Windows en la esquina inferior izquierda de la pantalla y seleccione Ejecutar. En el cuadro Abrir, escriba **regedit** y, a continuación, seleccione Aceptar.

2. Seleccione Sí cuando se le pida que permita al Editor del Registro realizar cambios en el dispositivo.

3. En el Editor del Registro, agregue un valor de cadena **de SharedComputerLicensing** con una configuración de 1 en HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. En el servidor RDS, ***inicie sesión como usuario*** final y compruebe que la activación del equipo compartido está habilitada para [Aplicaciones Microsoft 365 para empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Para obtener más información sobre los requisitos previos, las instrucciones de configuración y las instrucciones sobre instalaciones personalizadas mediante la herramienta de implementación de Office, consulte [Deploy Aplicaciones Microsoft 365 para empresas by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Para corregir errores relacionados con la activación de equipos compartidos, consulte Solucionar problemas con la activación del equipo compartido [para Aplicaciones Microsoft 365 para empresas](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  