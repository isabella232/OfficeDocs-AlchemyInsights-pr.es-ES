---
title: Solución de problemas de firma de certificados de SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529277"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="37e51-102">Solución de problemas de firma de certificados de SAML</span><span class="sxs-lookup"><span data-stu-id="37e51-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="37e51-103">Para resolver el problema del certificado de firma de SAML, siga los pasos recomendados:</span><span class="sxs-lookup"><span data-stu-id="37e51-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="37e51-104">Al agregar una aplicación empresarial que sea compatible con SSO, Azure generará un certificado denominado [Certificado de firma SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="37e51-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="37e51-105">Este certificado tiene una fecha de expiración de 3 años.</span><span class="sxs-lookup"><span data-stu-id="37e51-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="37e51-106">Para cambiar la fecha de expiración del certificado, vea [Personalizar la fecha de expiración del certificado de federación y extenderla a un nuevo certificado](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="37e51-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="37e51-107">Azure usará este certificado para firmar los tokens SAML solicitados por la aplicación y enviarlos a la aplicación para un SSO correcto.</span><span class="sxs-lookup"><span data-stu-id="37e51-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="37e51-108">Para que se complete, descargue el certificado desde Azure Portal y envíelo al proveedor de la aplicación para completar el proceso de SSO.</span><span class="sxs-lookup"><span data-stu-id="37e51-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="37e51-109">Cuando se complete este proceso, la aplicación confiará en este certificado y aceptará todos los tokens de SAML firmados con este certificado.</span><span class="sxs-lookup"><span data-stu-id="37e51-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="37e51-110">Si este certificado expira, cree uno nuevo, actualícelo en el proveedor de la aplicación y, después, actívelo en Azure.</span><span class="sxs-lookup"><span data-stu-id="37e51-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="37e51-111">Para obtener más información, consulte [Renovar un certificado que pronto expirará](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="37e51-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="37e51-112">Si el certificado expira, el usuario no se bloqueará.</span><span class="sxs-lookup"><span data-stu-id="37e51-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="37e51-113">[Agregue una dirección de correo electrónico para las notificaciones](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) que deba recibir antes de que expire el certificado actual.</span><span class="sxs-lookup"><span data-stu-id="37e51-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="37e51-114">El paso 4 es opcional.</span><span class="sxs-lookup"><span data-stu-id="37e51-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="37e51-115">Cambie las opciones de firma del certificado SAML de una aplicación y el algoritmo de firma de certificados.</span><span class="sxs-lookup"><span data-stu-id="37e51-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="37e51-116">Para obtener más información, consulte [Cambiar las opciones de firma de certificado y la firma del algoritmo](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="37e51-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

