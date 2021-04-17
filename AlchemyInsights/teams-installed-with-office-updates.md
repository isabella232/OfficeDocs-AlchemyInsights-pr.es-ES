---
title: Teams instalados con actualizaciones de Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 36b0b1a7bf37c27304b4124157dba9aba337678c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832399"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams instalado con actualizaciones de Office

Microsoft Teams se incluye  como parte de las nuevas instalaciones de Aplicaciones de Microsoft 365 para empresas, Aplicaciones de Microsoft 365 para empresas y Office para Mac. Para obtener más información, [vea ¿Cuándo empezará Microsoft Teams a incluirse con las nuevas instalaciones de Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Además, a partir de la versión 1906 en El  canal actual, Teams se agregará gradualmente a las instalaciones existentes de Aplicaciones de Microsoft 365 para empresas (y Aplicaciones de Microsoft 365 para empresas) en dispositivos que ejecutan Windows al actualizar la instalación existente a la versión más reciente. Para obtener más información, vea [¿Qué sucede con las instalaciones existentes de Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Nota:** Si no desea esperar a esta programación de lanzamiento, puede implementar Teams como independiente para los usuarios siguiendo estas instrucciones [o](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)puede hacer que los usuarios instalen Teams por sí mismos desde https://teams.microsoft.com/downloads .

Si su organización no está lista para implementar Teams, puede excluir ***Teams*** de instalaciones [nuevas](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) o [existentes](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) de Office. Si desea que Teams esté instalado, pero no quiere que Teams se inicie automáticamente para el usuario después de instalarlo, vea Impedir que [Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)se inicie automáticamente después de la instalación .

Para ***desinstalar Teams*** desde un dispositivo que ejecuta Windows, consulta Desinstalar Microsoft [Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). Para limpiar Microsoft Teams de varios usuarios o máquinas de destino, consulte [Limpieza de implementación de Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Si usa equipos compartidos, Servicios de Escritorio remoto (RDS) o Infraestructura de escritorio virtual (VDI), vea [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams). Si usa Office para Mac, vea [Instalaciones de Microsoft Teams en un Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Nota:** Después de instalar Teams, se actualiza [automáticamente](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) aproximadamente cada dos semanas con nuevas características y actualizaciones de calidad. 