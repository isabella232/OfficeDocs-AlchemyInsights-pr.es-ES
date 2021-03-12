---
title: DLP no funciona como se esperaba
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707827"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="fb04d-102">DLP no funciona como se esperaba</span><span class="sxs-lookup"><span data-stu-id="fb04d-102">DLP not working as expected</span></span>

<span data-ttu-id="fb04d-103">**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="fb04d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="fb04d-104">**Configuración de DLP**</span><span class="sxs-lookup"><span data-stu-id="fb04d-104">**Setting up DLP**</span></span>

<span data-ttu-id="fb04d-105">¿Tiene problemas con prevención de pérdida de datos **(DLP)** en Office 365 no funciona como se esperaba?</span><span class="sxs-lookup"><span data-stu-id="fb04d-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="fb04d-106">Si es así, asegúrese de que la directiva **DLP** está configurada correctamente y de que los datos contienen lo que la directiva **DLP** está buscando cuando se está evaluando.</span><span class="sxs-lookup"><span data-stu-id="fb04d-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="fb04d-107">Las directivas DLP le permiten identificar y proteger información confidencial en su organización.</span><span class="sxs-lookup"><span data-stu-id="fb04d-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="fb04d-108">Para configurar directivas DLP, use la información [aquí](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span><span class="sxs-lookup"><span data-stu-id="fb04d-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="fb04d-109">**Qué buscan las directivas DLP**</span><span class="sxs-lookup"><span data-stu-id="fb04d-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="fb04d-110">Al usar los **tipos de** información confidencial integrados en los centros de seguridad y cumplimiento, las directivas DLP buscan patrones y elementos específicos al detectar estos tipos confidenciales.</span><span class="sxs-lookup"><span data-stu-id="fb04d-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="fb04d-111">**Tipos de información confidencial integrados**</span><span class="sxs-lookup"><span data-stu-id="fb04d-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="fb04d-112">Para obtener información sobre los tipos confidenciales integrados y lo que busca una directiva DLP al detectar el tipo confidencial, vea: Qué buscan los tipos de información [confidencial](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="fb04d-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="fb04d-113">**Tipos de información confidencial personalizados**</span><span class="sxs-lookup"><span data-stu-id="fb04d-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="fb04d-114">Si está intentando crear tipos de información confidencial personalizados, use el siguiente artículo para obtener información sobre cómo crear un tipo confidencial personalizado: Crear un tipo de información [confidencial personalizada](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="fb04d-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="fb04d-115">**Probar una directiva DLP**</span><span class="sxs-lookup"><span data-stu-id="fb04d-115">**Test a DLP policy**</span></span>

<span data-ttu-id="fb04d-116">Para probar los datos con un tipo de información  confidencial integrada o personalizada, use la opción Tipo de prueba en **Clasificaciones**  >  **Tipos de información confidencial**.</span><span class="sxs-lookup"><span data-stu-id="fb04d-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="fb04d-117">Para obtener más información, vea [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="fb04d-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="fb04d-118">**Informes**</span><span class="sxs-lookup"><span data-stu-id="fb04d-118">**Reports**</span></span>
  
- <span data-ttu-id="fb04d-119">Obtenga información sobre datos confidenciales con [informes DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="fb04d-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="fb04d-120">Vea detalles específicos del evento con un [informe de incidentes](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="fb04d-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
