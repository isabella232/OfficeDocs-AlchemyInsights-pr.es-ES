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
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082959"
---
# <a name="authentication-app"></a>Aplicación de autenticación

Si es un administrador global, puede averiguar rápidamente lo que ha ocurrido o diagnosticar problemas relacionados con el inicio de sesión del usuario mediante el diagnóstico [de inicio de sesión](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. Para iniciar el diagnóstico, haga clic en el botón "[Iniciar diagnóstico".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Para buscar el evento que se va a analizar, escriba los detalles que tiene sobre el usuario, la aplicación, la hora de inicio de sesión, el identificador de solicitud o el identificador de correlación.
1. Revise los resultados del diagnóstico en los que se indican los detalles de lo sucedido y qué cambios puede realizar en caso necesario.

**Compruebe el escenario aplicable:**

1. Si un usuario no recibe una notificación de inserción en la aplicación Microsoft Authenticator, compruebe que no se muestran en los usuarios bloqueados de MFA como se describe en Bloquear y desbloquear [usuarios](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Si el usuario no está bloqueado para MFA pero no recibe una notificación de inserción, puede abrir la aplicación Microsoft Authenticator, que extraerá las solicitudes de aprobación pendientes.
1. Como método de inicio de sesión alternativo, el usuario también puede hacer clic en Iniciar sesión de otra forma y elegir usar un código de verificación desde mi aplicación móvil.
1. La Microsoft Authenticator app es el único método disponible para muchos usuarios. [Obtenga más información sobre los valores predeterminados de seguridad,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [consulte Authenticator Preguntas](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) frecuentes sobre la aplicación para las preguntas más frecuentes y cómo resolverlas.
 
**Vídeos recomendados**

[Cómo configurar la aplicación Authenticator en un teléfono nuevo (2 minutos).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
