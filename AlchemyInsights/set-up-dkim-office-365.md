---
title: Configuración DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808724"
---
# <a name="setup-dkim"></a><span data-ttu-id="07f98-102">Configuración DKIM</span><span class="sxs-lookup"><span data-stu-id="07f98-102">Setup DKIM</span></span>

<span data-ttu-id="07f98-103">[Aquí](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)se indican las instrucciones completas para configurar DKIM para los dominios personalizados en Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="07f98-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="07f98-104">Para **cada** dominio personalizado, debe crear **dos** registros CNAME de DKIM en el servicio de hospedaje de DNS de su dominio (normalmente, el registrador de dominios).</span><span class="sxs-lookup"><span data-stu-id="07f98-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="07f98-105">Por ejemplo, contoso.com y fourthcoffee.com requieren cuatro registros CNAME de DKIM: dos para contoso.com y dos para fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="07f98-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="07f98-106">Los registros CNAME de DKIM para **cada** dominio personalizado usan los siguientes formatos:</span><span class="sxs-lookup"><span data-stu-id="07f98-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="07f98-107">**Nombre de host**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="07f98-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="07f98-108">**Apunta a la dirección o al valor**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="07f98-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="07f98-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="07f98-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="07f98-110">**Nombre de host**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="07f98-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="07f98-111">**Apunta a la dirección o al valor**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="07f98-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="07f98-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="07f98-112">**TTL**: 3600</span></span>

   <span data-ttu-id="07f98-113">\<DomainGUID\> es el texto a la izquierda de `.mail.protection.outlook.com` en el registro MX personalizado para el dominio personalizado (por ejemplo, `contoso-com` para el dominio contoso.com).</span><span class="sxs-lookup"><span data-stu-id="07f98-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="07f98-114">\<InitialDomain\> es el dominio que usó cuando se suscribió a Microsoft 365 (por ejemplo, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="07f98-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="07f98-115">Una vez que haya creado los registros CNAME para sus dominios personalizados, siga las instrucciones siguientes:</span><span class="sxs-lookup"><span data-stu-id="07f98-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="07f98-116">a.</span><span class="sxs-lookup"><span data-stu-id="07f98-116">a.</span></span> <span data-ttu-id="07f98-117">[inicie sesión en Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) con su cuenta profesional o educativa.</span><span class="sxs-lookup"><span data-stu-id="07f98-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="07f98-118">b.</span><span class="sxs-lookup"><span data-stu-id="07f98-118">b.</span></span> <span data-ttu-id="07f98-119">Seleccione el icono del iniciador de aplicaciones en la esquina superior izquierda y elija **Administrador**.</span><span class="sxs-lookup"><span data-stu-id="07f98-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="07f98-120">c.</span><span class="sxs-lookup"><span data-stu-id="07f98-120">c.</span></span> <span data-ttu-id="07f98-121">En el panel de navegación inferior izquierdo, expanda **Administración** y elija **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="07f98-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="07f98-122">d.</span><span class="sxs-lookup"><span data-stu-id="07f98-122">d.</span></span> <span data-ttu-id="07f98-123">Vaya a **protección**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="07f98-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="07f98-124">e.</span><span class="sxs-lookup"><span data-stu-id="07f98-124">e.</span></span> <span data-ttu-id="07f98-125">Seleccione el dominio y, a continuación, elija **Habilitar** para **firmar mensajes para este dominio con firmas DKIM**.</span><span class="sxs-lookup"><span data-stu-id="07f98-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="07f98-126">Repita este paso para cada dominio personalizado.</span><span class="sxs-lookup"><span data-stu-id="07f98-126">Repeat this step for each custom domain.</span></span>
