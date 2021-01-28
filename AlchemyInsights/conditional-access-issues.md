---
title: Problemas de acceso condicional
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013980"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="495f4-102">Problemas de acceso condicional</span><span class="sxs-lookup"><span data-stu-id="495f4-102">Conditional access issues</span></span>

<span data-ttu-id="495f4-103">**Resolver problemas mediante el diagnóstico de inicio de sesión**</span><span class="sxs-lookup"><span data-stu-id="495f4-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="495f4-104">Puede averiguar rápidamente qué ha ocurrido o diagnosticar problemas relacionados con el inicio de sesión del usuario mediante el diagnóstico [de inicio de sesión:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="495f4-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="495f4-105">Inicie el diagnóstico de inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="495f4-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="495f4-106">Busque el evento que se va a analizar especificando los detalles que tiene sobre el usuario, la aplicación, la hora de inicio de sesión, el identificador de solicitud o el identificador de correlación.</span><span class="sxs-lookup"><span data-stu-id="495f4-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="495f4-107">Revise los resultados de diagnóstico que muestran los detalles de lo que ha ocurrido y las acciones que puede realizar para realizar cambios (si es necesario).</span><span class="sxs-lookup"><span data-stu-id="495f4-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="495f4-108">**Pasos para solucionar problemas de un inicio de sesión**</span><span class="sxs-lookup"><span data-stu-id="495f4-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="495f4-109">Vaya a la página de inicio de sesión de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="495f4-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="495f4-110">Filtra los inicios de sesión por usuario, intervalo de tiempo, aplicación, estado, aplicación cliente, entre otros.</span><span class="sxs-lookup"><span data-stu-id="495f4-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="495f4-111">Seleccione un evento de inicio de sesión y vea la pestaña Acceso condicional para ver qué directivas se evaluaron.</span><span class="sxs-lookup"><span data-stu-id="495f4-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="495f4-112">Haga clic en la fila de una directiva para ver los detalles de la directiva y comprender por qué se aplicó.</span><span class="sxs-lookup"><span data-stu-id="495f4-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="495f4-113">**Herramientas para solucionar problemas de una directiva de acceso condicional**</span><span class="sxs-lookup"><span data-stu-id="495f4-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="495f4-114">El modo de solo informe le permite evaluar una directiva sin afectar a los usuarios.</span><span class="sxs-lookup"><span data-stu-id="495f4-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="495f4-115">La herramienta what-if le permite simular eventos de inicio de sesión y ver qué directivas se aplican.</span><span class="sxs-lookup"><span data-stu-id="495f4-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="495f4-116">La información y el libro de informes muestran el impacto en tiempo real de cada directiva.</span><span class="sxs-lookup"><span data-stu-id="495f4-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="495f4-117">**Directivas de protección de línea base**</span><span class="sxs-lookup"><span data-stu-id="495f4-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="495f4-118">Las directivas de protección de línea base han quedado en desuso.</span><span class="sxs-lookup"><span data-stu-id="495f4-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="495f4-119">Ya no se aplican y pronto se quitarán de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="495f4-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="495f4-120">Se recomienda habilitar los [valores predeterminados de seguridad.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="495f4-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="495f4-121">Para obtener más información sobre el acceso condicional, vea:</span><span class="sxs-lookup"><span data-stu-id="495f4-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="495f4-122">[Procedimientos recomendados para el acceso condicional en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condiciones en el acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controles en el acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Ubicaciones en el acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="495f4-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
