---
title: Obtener una lista de aplicaciones empresariales
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379914"
---
# <a name="get-a-list-of-enterprise-applications"></a>Obtener una lista de aplicaciones empresariales

1. Para **obtener una lista** de aplicaciones empresariales (todas las aplicaciones o filtradas por nombre para mostrar, identificador, URI de identificador, etc.) mediante el comando de Powershell, vea [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Para obtener una lista de objetos de entidad de servicio (todos los objetos o filtrados por identificador) mediante el comando de Powershell, vea [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Si desea obtener una lista de aplicaciones **configuradas con SAML,** los siguientes scripts de PowerShell pueden ayudarle:

    Cada aplicación Application sea una aplicación OAuth o una aplicación SAML (tanto las aplicaciones de galería como las que no son de galería) tendrían dos objetos creados en AAD cuando se produce su registro. Uno se denomina objeto Application y el otro es el objeto de entidad de servicio. Al volcar las propiedades de un objeto de entidad de seguridad de servicio mediante PowerShell, encontrará que cada aplicación tiene un número determinado de etiquetas asociadas como:

    - Las aplicaciones de OAuth tendrían una etiqueta denominada "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Las aplicaciones SAML que no son de galería tendrían una etiqueta denominada "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Por lo tanto, puedes usar estas etiquetas y averiguar qué tipo de aplicación es. La etiqueta "**WindowsAzureActiveDirectoryIntegratedApp**" es común a todos los tipos de aplicaciones. Puedes usar el siguiente fragmento de código para enumerar todas las aplicaciones SAML (tanto de galería como de no galería):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Para obtener más información, vea [Identificar aplicaciones habilitadas para SAML en Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Buscar y enumerar solo aplicaciones web:** use el siguiente comando para obtener todas las aplicaciones de Azure AD con el tipo de aplicación "Aplicación web/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Buscar y enumerar aplicaciones nativas por sí solas:** ejecute el siguiente comando para obtener todas las aplicaciones de cliente nativo (dispositivo móvil o de escritorio).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Exportar todos los detalles de la aplicación de Azure AD** registrada a CSV: el siguiente comando exporta todas las aplicaciones de Azure AD con los detalles necesarios al archivo csv:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Necesidad de exportar una lista de aplicaciones de Azure** sin usar: informe de auditoría

    Azure AD puede mostrar registros de aplicaciones solo durante 30 días siempre que tenga licencia de Azure AD Premium.
    Tiene dos opciones para conservar los datos durante más de 30 días. Puede usar las API de Informes de [Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) para recuperar los datos mediante programación y almacenarlos en una base de datos. Como alternativa, puede integrar registros de auditoría en un sistema SIEM de terceros.

    También puede descargar la lista de aplicaciones para todas las aplicaciones y aplicaciones de propiedad en Azure Active Directory>Registros de aplicaciones>Descargar>todas las aplicaciones/aplicaciones de propiedad.

    Para obtener una lista de aplicaciones a través de MS Graph, vea Enumerar aplicaciones [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) y tipo de recurso de aplicación [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
