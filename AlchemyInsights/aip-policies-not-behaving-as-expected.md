---
title: 'AIP: las directivas no se comportan como se esperaba'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580782"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="03ecc-102">AIP: las directivas no se comportan como se esperaba</span><span class="sxs-lookup"><span data-stu-id="03ecc-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="03ecc-103">Azure Information Protection: las directivas no se comportan como se esperaba. Consulte el texto a continuación para obtener instrucciones recomendadas para diferentes aspectos de directiva:</span><span class="sxs-lookup"><span data-stu-id="03ecc-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="03ecc-104">Si tiene problemas con las marcas visuales, consulte [Cuando se aplican marcas visuales](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="03ecc-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="03ecc-105">Si tiene problemas con el etiquetado automático, consulte [Cómo configurar las condiciones de la clasificación automática y recomendada para Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) y [¿Qué intentan detectar los tipos de información confidencial?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="03ecc-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="03ecc-106">Si tiene problemas con la protección Nativa/Pfile, consulte [Configuración de la API de archivo](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="03ecc-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="03ecc-107">Compruebe si usa directivas de ámbito que no están correctamente configuradas: [Cómo configurar la directiva de Azure Information Protection para determinados usuarios al usar las directivas de ámbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="03ecc-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="03ecc-108">Si el etiquetado automático no funciona para Outlook cuando se adjunte un documento etiquetado, compruebe que DRMEncryptProperty no se ha definido como se describe a continuación: [Configuración del registro de IRM para seguridad](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="03ecc-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="03ecc-109">Si sigue experimentando problemas, recopile los registros de los clientes de Azure Information Protection y adjunte los registros exportados a este vale.</span><span class="sxs-lookup"><span data-stu-id="03ecc-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="03ecc-110">Abra un documento de Office o cree un nuevo correo electrónico en Outlook.</span><span class="sxs-lookup"><span data-stu-id="03ecc-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="03ecc-111">Haga clic en **Proteger/Confidencialidad** > **Ayuda y comentarios**.</span><span class="sxs-lookup"><span data-stu-id="03ecc-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="03ecc-112">Haga clic en **Exportar registros**.</span><span class="sxs-lookup"><span data-stu-id="03ecc-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="03ecc-113">Guarde los registros en la ubicación que desee y adjúntelos a esta solicitud de servicio.</span><span class="sxs-lookup"><span data-stu-id="03ecc-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="03ecc-114">Recursos adicionales:</span><span class="sxs-lookup"><span data-stu-id="03ecc-114">Additional resources:</span></span>

- [<span data-ttu-id="03ecc-115">Cómo configurar una etiqueta para las marcas visuales de Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="03ecc-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="03ecc-116">Revisar la documentación de Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="03ecc-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="03ecc-117">Usar las etiquetas de confidencialidad en Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="03ecc-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

