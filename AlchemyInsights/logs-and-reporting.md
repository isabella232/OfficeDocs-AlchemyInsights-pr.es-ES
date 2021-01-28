---
title: Registros e informes
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031507"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="88aac-102">Registros e informes</span><span class="sxs-lookup"><span data-stu-id="88aac-102">Logs and Reporting</span></span>

<span data-ttu-id="88aac-103">[Las preguntas más frecuentes sobre informes](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) de Azure Active Directory responden a las preguntas más frecuentes sobre los informes de Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="88aac-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="88aac-104">Para obtener más información, [vea informes de Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="88aac-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="88aac-105">**Solución de problemas con auditoría**</span><span class="sxs-lookup"><span data-stu-id="88aac-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="88aac-106">Si tiene problemas para ver algunas actividades de auditoría y la actividad que falta está en esta [lista,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)envíe un vale de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="88aac-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="88aac-107">Si tiene problemas para ver los registros de auditoría en su espacio empresarial, envíe un vale de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="88aac-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="88aac-108">Si las actividades de auditoría no se muestran inmediatamente [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) en Azure Portal, consulte nuestra información de latencia y presente un vale de soporte técnico si el retraso supera la latencia documentada.</span><span class="sxs-lookup"><span data-stu-id="88aac-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="88aac-109">Retención de registros de actividad de Azure AD</span><span class="sxs-lookup"><span data-stu-id="88aac-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="88aac-110">Si no ve toda la auditoría del intervalo de fechas seleccionado, puede descargar hasta 250.000 filas (ordenadas por las más recientes) de inicios de sesión desde Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="88aac-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="88aac-111">Para obtener más información, vea [La descarga de actividades de auditoría.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="88aac-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="88aac-112">**Solución de problemas con inicios de sesión**</span><span class="sxs-lookup"><span data-stu-id="88aac-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="88aac-113">Solo puedes ver los últimos 30 días de datos si tienes una licencia de Azure AD Premium (P1 o P2) para tu espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="88aac-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="88aac-114">Los inicios de sesión solo están disponibles para los inquilinos de Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="88aac-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="88aac-115">No está disponible para inquilinos con licencia gratuita o básica.</span><span class="sxs-lookup"><span data-stu-id="88aac-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="88aac-116">Si su espacio empresarial tiene una licencia Premium P1 y no puede [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) ver los inicios de sesión, consulte nuestra información de latencia y presente un vale de soporte técnico si el retraso supera la latencia documentada.</span><span class="sxs-lookup"><span data-stu-id="88aac-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="88aac-117">Si no ve todos los inicios de sesión del intervalo de fechas seleccionado, tenga en cuenta que puede descargar hasta 250.000 filas (ordenadas por las más recientes) de inicios de sesión desde Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="88aac-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="88aac-118">Para obtener más información, vea [la descarga de actividades de inicio de sesión.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="88aac-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="88aac-119">**Solucionar problemas de informes de seguridad (usuarios marcados como de riesgo, inicio de sesión arriesgado)**</span><span class="sxs-lookup"><span data-stu-id="88aac-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="88aac-120">Usuarios marcados para el informe de seguridad de riesgos</span><span class="sxs-lookup"><span data-stu-id="88aac-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="88aac-121">Informe de inicios de sesión de riesgo en el portal de Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="88aac-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="88aac-122">Eventos de riesgo de Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="88aac-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
