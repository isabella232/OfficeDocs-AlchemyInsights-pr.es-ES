---
title: Errores en el inicio de sesión de usuario
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886890"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="1f492-102">Errores en el inicio de sesión de usuario</span><span class="sxs-lookup"><span data-stu-id="1f492-102">User sign-in errors</span></span>

<span data-ttu-id="1f492-103">**Resolver problemas mediante el diagnóstico de inicio de sesión**</span><span class="sxs-lookup"><span data-stu-id="1f492-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="1f492-104">Para diagnosticar problemas relacionados con el inicio de sesión de usuario o detectar su causa, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="1f492-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="1f492-105">Inicie el [diagnóstico de inicio de sesión](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="1f492-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="1f492-106">Busque el evento que desea analizar especificando los detalles que tiene sobre el usuario, la aplicación, la hora de inicio de sesión, el id. de solicitud o el id. de correlación.</span><span class="sxs-lookup"><span data-stu-id="1f492-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="1f492-107">Revise los resultados del diagnóstico en los que se indican los detalles de lo sucedido y qué cambios puede realizar en caso necesario.</span><span class="sxs-lookup"><span data-stu-id="1f492-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="1f492-108">**¿Busca información sobre los códigos de error que devuelve el servicio de token de seguridad (STS) de Azure Active Directory (Azure AD)?**</span><span class="sxs-lookup"><span data-stu-id="1f492-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="1f492-109">Consulte [este artículo](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) para buscar descripciones, correcciones y algunas sugerencias de soluciones alternativas sobre los errores AADST</span><span class="sxs-lookup"><span data-stu-id="1f492-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>