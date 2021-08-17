---
title: Buscar aplicaciones que faltan en la hoja Registro de aplicaciones
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057119"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Buscar aplicaciones que faltan en la hoja Registro de aplicaciones

1. No se pueden encontrar aplicaciones en el portal de registro de aplicaciones.

    Si una aplicación es una aplicación multiinquilino y se registró en otro inquilino, no se mostrará en la hoja Registro de aplicaciones. Sin embargo, puede encontrarla en la hoja Enterprise aplicaciones una vez que se haya accedido a ella (después de haber sido consentida) y se haya creado la entidad de servicio en el espacio empresarial. Para obtener más información, [vea Apps & service principals in Azure AD - Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. No se pueden ver aplicaciones en la hoja Registro de aplicaciones aunque seas administrador.

    Asegúrese de que está en el directorio correcto en Azure Portal.
3. Mi aplicación no aparece en la hoja Enterprise aplicaciones, pero se muestra cuando se consulta el comando de PowerShell.

    A veces, después de eliminar la aplicación de Azure Portal, no aparece en el portal, pero puede que no se haya eliminado por completo. Para obtener más información, vea:
    - Puede recuperar la lista de aplicaciones eliminadas anteriormente y ver si la aplicación aparece en la lista mediante el comando de Powershell: **Get-AzureADDeletedApplication**. Para obtener más información, [vea Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Si desea quitar la aplicación por completo, puede probar lo siguiente en PowerShell: **Remove-AzureADApplication -ObjectId**. Para obtener más información, [vea Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Como alternativa, puede intentar restaurar la aplicación eliminada mediante el siguiente comando de Powershell: **Restaurar AzureADDeletedApplication -ObjectId**. Para obtener más información, [vea Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. No se puede encontrar una lista de todas las aplicaciones empresariales preinstaladas en mi nuevo inquilino de Azure.

    De forma predeterminada, no hay aplicaciones empresariales preinstaladas en Azure AD. Debe agregarlo manualmente desde la opción "Nueva aplicación" explorando desde la galería de Azure AD o agregando una aplicación que no sea de galería. Para obtener más información, vea Inicio rápido: Agregar una aplicación al [inquilino de Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Si eres un administrador global, puedes acceder fácilmente a tus aplicaciones mediante el Microsoft 365 [app Selector](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. No se pueden encontrar mis aplicaciones en el portal de Mis aplicaciones.

    Asegúrate de que las aplicaciones no estén ocultas en la página de la colección Mis aplicaciones. Para obtener más información, vea [Colecciones (versión preliminar) en El portal de Mis aplicaciones : Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Para iniciar aplicaciones desde el portal de Mis [aplicaciones, consulte Localizar & usar aplicaciones](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)en el portal de Mis aplicaciones - Azure AD .
7. Office 365 Mover app is not showing up on Enterprise Applications blade after installation.

    La aplicación "Office 365 Mover" es una aplicación de varios usuarios que no necesita agregarse a AAD mediante la sección Aplicaciones de galería en Enterprise registro de aplicaciones. Para acceder Office 365 mover, simplemente inicie sesión en la aplicación y pediría el consentimiento del usuario para los permisos. Una vez que el usuario proporciona el consentimiento, esta aplicación se agregará automáticamente al inquilino con el identificador de correo electrónico que haya iniciado sesión.

    Después de iniciar sesión en la aplicación, debería poder encontrar la entrada de esta aplicación en la hoja Enterprise aplicaciones de AAD. Debes buscar esa aplicación escribiendo el nombre completo, es decir, "Office 365 Mover" o simplemente busca en "office" y debería enumerar la aplicación. Para obtener más información, [vea Office 365 Mover indica](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)que ya está instalado, pero no aparece en la Enterprise application gallery .
8. Inicio rápido: ver la lista de aplicaciones que usan el inquilino de [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) para la administración de identidades muestra cómo ver las aplicaciones, también conocidas como aplicaciones, que ya están configuradas para usar el inquilino de Azure AD como su proveedor de identidades (IdP).
9. [Solucionar problemas comunes al agregar o](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) quitar una aplicación a Azure Active Directory ayuda a comprender los problemas comunes a los que se enfrentan las personas al ver aplicaciones en Azure Active Directory.
