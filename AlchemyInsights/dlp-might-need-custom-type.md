---
title: Es posible que DLP necesite un tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507531"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="2ce27-102">Es posible que DLP necesite un tipo personalizado</span><span class="sxs-lookup"><span data-stu-id="2ce27-102">DLP might need a custom type</span></span>

<span data-ttu-id="2ce27-103">**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="2ce27-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2ce27-104">**Es posible que DLP requiera un tipo de información personalizada**</span><span class="sxs-lookup"><span data-stu-id="2ce27-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="2ce27-105">Con una directiva de prevención de pérdida de datos (DLP), puede identificar y proteger los datos confidenciales de su organización.</span><span class="sxs-lookup"><span data-stu-id="2ce27-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="2ce27-106">En algunos escenarios, es posible que necesite crear su propio tipo **personalizado** de información confidencial para proteger los datos de su organización.</span><span class="sxs-lookup"><span data-stu-id="2ce27-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="2ce27-107">Por ejemplo, es posible que su organización necesite identificar y proteger los identificadores de los empleados u otros datos en algún formato específico de su organización. Si es así, consulte los artículos siguientes para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="2ce27-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="2ce27-108">**Personalizar un tipo de información confidencial integrado**</span><span class="sxs-lookup"><span data-stu-id="2ce27-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="2ce27-109">Si un tipo de información confidencial incorporado satisface sus necesidades con solo unos cuantos ajustes, puede [personalizar un tipo de información confidencial integrada](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="2ce27-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="2ce27-110">Por ejemplo, puede Agregar o quitar palabras clave, o bien agregar o quitar evidencias auxiliares, como una fecha o una dirección.</span><span class="sxs-lookup"><span data-stu-id="2ce27-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="2ce27-111">**Crear un tipo personalizado de información confidencial**</span><span class="sxs-lookup"><span data-stu-id="2ce27-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="2ce27-112">Pero si necesita identificar y proteger por completo un tipo diferente de información confidencial, puede [crear un tipo personalizado de información confidencial](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) en la interfaz de usuario del centro de seguridad & cumplimiento.</span><span class="sxs-lookup"><span data-stu-id="2ce27-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="2ce27-113">**Crear un tipo personalizado de información confidencial en PowerShell del Centro de seguridad y cumplimientol**</span><span class="sxs-lookup"><span data-stu-id="2ce27-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="2ce27-114">Por último, si la interfaz de usuario no proporciona todas las opciones que necesita, puede [crear un tipo personalizado de información confidencial en el PowerShell del centro de cumplimiento de & de seguridad](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="2ce27-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="2ce27-115">Al comenzar con un archivo XML, puede usar todas las opciones disponibles.</span><span class="sxs-lookup"><span data-stu-id="2ce27-115">By starting with an XML file, you can use every option available.</span></span>
