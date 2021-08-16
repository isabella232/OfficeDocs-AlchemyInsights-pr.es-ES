---
title: Teams instalado con Office actualizaciones
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
ms.openlocfilehash: c473a001d1441362baad9feb44323b46f1cef42d3c431ef87f0fb0172f10d152
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048749"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams instalado con Office actualizaciones

Microsoft Teams se incluye como parte de las nuevas ***instalaciones*** de Aplicaciones Microsoft 365 para empresas, Aplicaciones Microsoft 365 para negocios y Office para Mac. Para obtener más información, vea [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Además, a partir de la versión 1906 en el canal actual, Teams se agregará gradualmente a las instalaciones existentes de Aplicaciones Microsoft 365 para empresas (y Aplicaciones Microsoft 365 para negocios) en dispositivos que ejecutan Windows al actualizar la instalación existente a la versión más reciente.  Para obtener más información, vea [¿Qué sucede con las instalaciones existentes de Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Nota:** Si no desea esperar a esta programación de lanzamiento, puede implementar Teams como independiente para los usuarios siguiendo estas [instrucciones,](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)o puede hacer que los usuarios instalen Teams ellos mismos desde https://teams.microsoft.com/downloads .

Si su organización no está lista para implementar Teams, puede [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) excluir [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Teams de instalaciones nuevas o existentes de Office.  Si desea Teams que se instale, pero no desea que Teams se inicie automáticamente para el usuario después de instalarlo, vea Impedir que [Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)se inicie automáticamente después de la instalación .

Para ***desinstalar Teams*** desde un dispositivo que se Windows, consulta Desinstalar [Microsoft Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). Para limpiar los Microsoft Teams de varios usuarios o máquinas de destino, [consulte Microsoft Teams limpieza de implementación](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Si usa equipos compartidos, Servicios de Escritorio remoto (RDS) o Infraestructura de escritorio virtual (VDI), vea [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams). Si usas Office para Mac, consulta [Microsoft Teams instalaciones en mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Nota:** Después Teams se instala, se actualiza [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) automáticamente aproximadamente cada dos semanas con nuevas características y actualizaciones de calidad. 