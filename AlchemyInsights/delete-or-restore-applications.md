---
title: Eliminar o restaurar aplicaciones
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013986"
---
# <a name="delete-or-restore-applications"></a>Eliminar o restaurar aplicaciones

**Para eliminar una aplicación del inquilino de Azure AD:**

1. En el **portal de Azure AD,** seleccione **Aplicaciones de empresa.** A continuación, busque y seleccione la aplicación que desea eliminar.
2. En la **sección** Administrar del panel izquierdo, seleccione **Propiedades**.
3. Seleccione **Eliminar** y, a continuación, seleccione **Sí** para confirmar que desea eliminar la aplicación del inquilino de Azure AD.

Para obtener más información sobre cómo eliminar una aplicación, vea Inicio rápido: Eliminar una aplicación de su inquilino de [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

En PowerShell, el cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) quita las configuraciones de Proxy de aplicación de una aplicación específica en Azure Active Directory y puede eliminar la aplicación por completo si se especifica.

Puede restaurar **una aplicación eliminada con** PowerShell. Una vez identificada la aplicación que desea restaurar, puede restaurarla con [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
