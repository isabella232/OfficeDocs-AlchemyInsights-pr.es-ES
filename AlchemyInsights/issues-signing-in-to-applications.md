---
title: Problemas al iniciar sesión en las aplicaciones
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
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886904"
---
# <a name="issues-signing-in-to-applications"></a>Problemas al iniciar sesión en las aplicaciones

Para detectar la causa o diagnosticar problemas relacionados con el inicio de sesión del usuario, siga los siguientes pasos:

1. Inicie el [Diagnóstico de inicio de sesión](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Busque el evento que desea analizar especificando los detalles que tiene acerca del usuario, la aplicación, la hora de inicio de sesión, el id. de solicitud o el id. de correlación.
3. Revise los resultados del diagnóstico en los que se mostrarán los detalles de lo ocurrido, así como las acciones que puede realizar para hacer cambios, de ser necesario.

Estos son algunos problemas comunes que podría experimentar al iniciar sesión en las aplicaciones:

1. Usted o el usuario **completaron el inicio de sesión en Azure AD, pero ven un aviso inesperado**: Consulte los artículos [Solicitud de consentimiento inesperado al iniciar sesión en una aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) y [Error inesperado al realizar el consentimiento en una aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Usted o un usuario **iniciaron sesión directamente en una aplicación, pero no pueden hacerlo desde ningún vínculo profundo en el portal personalizado o en el panel de acceso**: Consulte [Solucionar problemas al iniciar sesión en una aplicación desde My Apps en Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Usted o un usuario **completaron el inicio de sesión en Azure AD, pero la aplicación muestra un mensaje de error y no permite al usuario finalizar el flujo de inicio de sesión**: El problema es que la aplicación no acepta la respuesta que emitió Azure AD. Siga [estos pasos](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) para solucionar el problema.
4. Usted o un usuario **tienen problemas para iniciar sesión en una de las aplicaciones fuera de la galería pero que está configurada para el inicio de sesión único con contraseña**: Siga las instrucciones en [estos pasos](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) para solucionar el problema.
5. Usted o un usuario **tienen problemas para iniciar sesión en una aplicación de la galería de Azure AD configurada para el inicio de sesión único con contraseña**: Siga [estos pasos](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) para solucionar el problema.
6. Usted o un usuario **tienen problemas para iniciar sesión en una aplicación de Microsoft**: Siga [estos pasos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) para solucionar el problema.
7. Usted o un usuario **tienen problemas para iniciar sesión en una aplicación fuera de la galería configurada para el inicio de sesión único federado**: Siga [estos pasos](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) para solucionar el problema.
8. Usted o un usuario **tienen problemas para iniciar sesión en una aplicación de la galería de Azure AD configurada para el inicio de sesión único federado**: Siga [estos pasos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) para solucionar el problema.
9. Usted o un usuario **tienen problemas para iniciar sesión en una aplicación desarrollada de forma personalizada**: Siga [estos pasos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) para solucionar el problema.
10. Usted o un usuario **tienen problemas para iniciar sesión en una aplicación local con el proxy de la aplicación de Azure AD**: Siga [estos pasos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) para solucionar el problema.

