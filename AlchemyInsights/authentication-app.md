---
title: Aplicación de autenticación
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403839"
---
# <a name="authentication-app"></a><span data-ttu-id="dc341-102">Aplicación de autenticación</span><span class="sxs-lookup"><span data-stu-id="dc341-102">Authentication app</span></span>

<span data-ttu-id="dc341-103">Si es un administrador global, puede averiguar rápidamente lo que ha ocurrido o diagnosticar problemas relacionados con el inicio de sesión del usuario mediante el diagnóstico [de inicio de sesión](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="dc341-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="dc341-104">Para iniciar el diagnóstico, haga clic en el botón "[Iniciar diagnóstico".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="dc341-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="dc341-105">Para buscar el evento que se va a analizar, escriba los detalles que tiene sobre el usuario, la aplicación, la hora de inicio de sesión, el identificador de solicitud o el identificador de correlación.</span><span class="sxs-lookup"><span data-stu-id="dc341-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="dc341-106">Revise los resultados del diagnóstico en los que se indican los detalles de lo sucedido y qué cambios puede realizar en caso necesario.</span><span class="sxs-lookup"><span data-stu-id="dc341-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="dc341-107">**Compruebe el escenario aplicable:**</span><span class="sxs-lookup"><span data-stu-id="dc341-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="dc341-108">Si un usuario no recibe una notificación de inserción en la aplicación Microsoft Authenticator, compruebe que no se muestran en los usuarios bloqueados de MFA como se describe en Bloquear y [desbloquear usuarios.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="dc341-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="dc341-109">Si el usuario no está bloqueado para MFA pero no recibe una notificación de inserción, puede abrir la aplicación Microsoft Authenticator, que extraerá las solicitudes de aprobación pendientes.</span><span class="sxs-lookup"><span data-stu-id="dc341-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="dc341-110">Como método de inicio de sesión alternativo, el usuario también puede hacer clic en Iniciar sesión de otra forma y elegir usar un código de verificación desde mi aplicación móvil.</span><span class="sxs-lookup"><span data-stu-id="dc341-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="dc341-111">La aplicación Microsoft Authenticator es el único método disponible para muchos usuarios.</span><span class="sxs-lookup"><span data-stu-id="dc341-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="dc341-112">[Obtén más información sobre los valores predeterminados de seguridad,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)consulta Preguntas más frecuentes sobre la aplicación [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) para ver las preguntas más frecuentes y cómo resolverlas.</span><span class="sxs-lookup"><span data-stu-id="dc341-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="dc341-113">**Vídeos recomendados**</span><span class="sxs-lookup"><span data-stu-id="dc341-113">**Recommended Videos**</span></span>

<span data-ttu-id="dc341-114">[Cómo configurar la aplicación Authenticator en un teléfono nuevo (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="dc341-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
