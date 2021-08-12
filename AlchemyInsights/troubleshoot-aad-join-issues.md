---
title: Solucionar problemas de unión de Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939936"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Solucionar problemas de unión de Azure AD

1. Si configura los registros de dispositivos por primera vez, asegúrese de que ha revisado Introducción a la administración de dispositivos en [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) que le guiará sobre cómo obtener dispositivos bajo el control de Azure AD. 
1. Si vas a registrar dispositivos en Azure AD directamente e inscribirlos en Intune, deberás asegurarte de haber configurado [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) y tener las licencias [en](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) primer lugar.
1. Asegúrese de que está autorizado a realizar operaciones en Azure AD. Solo un administrador global de Azure AD puede administrar la configuración de registros de dispositivos.
1. Para realizar la implementación de unirse a Azure AD, vea [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Para obtener más información sobre cómo resolver problemas comunes con la unión a Azure AD, consulte Preguntas más frecuentes sobre unirse Windows 10 [Azure Ad](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) y para un dispositivo profesional, vea Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - [Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
