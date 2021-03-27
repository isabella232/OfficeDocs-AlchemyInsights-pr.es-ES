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
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="9fd2a-102">Obtener una lista de aplicaciones empresariales</span><span class="sxs-lookup"><span data-stu-id="9fd2a-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="9fd2a-103">Para **obtener una lista** de aplicaciones empresariales (todas las aplicaciones o filtradas por nombre para mostrar, identificador, URI de identificador, etc.) mediante el comando de Powershell, vea [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="9fd2a-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="9fd2a-104">Para obtener una lista de objetos de entidad de servicio (todos los objetos o filtrados por identificador) mediante el comando de Powershell, vea [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="9fd2a-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="9fd2a-105">Si desea obtener una lista de aplicaciones **configuradas con SAML,** los siguientes scripts de PowerShell pueden ayudarle:</span><span class="sxs-lookup"><span data-stu-id="9fd2a-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="9fd2a-106">Cada aplicación Application sea una aplicación OAuth o una aplicación SAML (tanto las aplicaciones de galería como las que no son de galería) tendrían dos objetos creados en AAD cuando se produce su registro.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="9fd2a-107">Uno se denomina objeto Application y el otro es el objeto de entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="9fd2a-108">Al volcar las propiedades de un objeto de entidad de seguridad de servicio mediante PowerShell, encontrará que cada aplicación tiene un número determinado de etiquetas asociadas como:</span><span class="sxs-lookup"><span data-stu-id="9fd2a-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="9fd2a-109">Las aplicaciones de OAuth tendrían una etiqueta denominada "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="9fd2a-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="9fd2a-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="9fd2a-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="9fd2a-111">Las aplicaciones SAML que no son de galería tendrían una etiqueta denominada "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="9fd2a-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="9fd2a-112">Por lo tanto, puedes usar estas etiquetas y averiguar qué tipo de aplicación es.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="9fd2a-113">La etiqueta "**WindowsAzureActiveDirectoryIntegratedApp**" es común a todos los tipos de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="9fd2a-114">Puedes usar el siguiente fragmento de código para enumerar todas las aplicaciones SAML (tanto de galería como de no galería):</span><span class="sxs-lookup"><span data-stu-id="9fd2a-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="9fd2a-115">Para obtener más información, vea [Identificar aplicaciones habilitadas para SAML en Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="9fd2a-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="9fd2a-116">**Buscar y enumerar solo aplicaciones web:** use el siguiente comando para obtener todas las aplicaciones de Azure AD con el tipo de aplicación "Aplicación web/API"</span><span class="sxs-lookup"><span data-stu-id="9fd2a-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="9fd2a-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="9fd2a-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="9fd2a-118">**Buscar y enumerar aplicaciones nativas por sí solas:** ejecute el siguiente comando para obtener todas las aplicaciones de cliente nativo (dispositivo móvil o de escritorio).</span><span class="sxs-lookup"><span data-stu-id="9fd2a-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="9fd2a-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="9fd2a-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="9fd2a-120">**Exportar todos los detalles de la aplicación de Azure AD** registrada a CSV: el siguiente comando exporta todas las aplicaciones de Azure AD con los detalles necesarios al archivo csv:</span><span class="sxs-lookup"><span data-stu-id="9fd2a-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="9fd2a-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="9fd2a-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="9fd2a-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="9fd2a-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="9fd2a-123">**Necesidad de exportar una lista de aplicaciones de Azure** sin usar: informe de auditoría</span><span class="sxs-lookup"><span data-stu-id="9fd2a-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="9fd2a-124">Azure AD puede mostrar registros de aplicaciones solo durante 30 días siempre que tenga licencia de Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="9fd2a-125">Tiene dos opciones para conservar los datos durante más de 30 días.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="9fd2a-126">Puede usar las API de Informes de [Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) para recuperar los datos mediante programación y almacenarlos en una base de datos.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="9fd2a-127">Como alternativa, puede integrar registros de auditoría en un sistema SIEM de terceros.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="9fd2a-128">También puede descargar la lista de aplicaciones para todas las aplicaciones y aplicaciones de propiedad en Azure Active Directory>Registros de aplicaciones>Descargar>todas las aplicaciones/aplicaciones de propiedad.</span><span class="sxs-lookup"><span data-stu-id="9fd2a-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="9fd2a-129">Para obtener una lista de aplicaciones a través de MS Graph, vea Enumerar aplicaciones [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) y tipo de recurso de aplicación [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="9fd2a-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
