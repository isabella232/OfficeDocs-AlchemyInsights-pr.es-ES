---
title: No se ha configurado el certificado de inserción de Apple MDM
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716874"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="da794-102">No se ha configurado el certificado de inserción de Apple MDM</span><span class="sxs-lookup"><span data-stu-id="da794-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="da794-103">No se ha configurado un certificado de inserción de MDM de Apple (también conocido como certificado de servicio de notificaciones push de Apple o APNs) en su suscripción.</span><span class="sxs-lookup"><span data-stu-id="da794-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="da794-104">Si no se ha configurado un certificado de inserción de MDM de Apple, no podrá inscribir y administrar los dispositivos iOS y MacOS.</span><span class="sxs-lookup"><span data-stu-id="da794-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="da794-105">Después de agregar el certificado a Intune, los usuarios pueden instalar la aplicación del portal de la empresa para inscribir sus dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="da794-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="da794-106">Seleccione **"Acepto".**</span><span class="sxs-lookup"><span data-stu-id="da794-106">Select **"I agree."**</span></span> <span data-ttu-id="da794-107">para conceder permiso a Microsoft para enviar datos a Apple.</span><span class="sxs-lookup"><span data-stu-id="da794-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="da794-108">Seleccione **Descargar al CSR** la solicitud de firma de certificado Intune necesaria para crear un certificado de inserción de Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="da794-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="da794-109">El archivo se usa para solicitar un certificado de relación de confianza del portal de certificados de inserción de Apple.</span><span class="sxs-lookup"><span data-stu-id="da794-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="da794-110">Seleccione **Crear el certificado de inserción de MDM** ir al portal de certificados de inserción de Apple.</span><span class="sxs-lookup"><span data-stu-id="da794-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="da794-111">Inicie sesión con el ID. de Apple de su empresa y, a continuación, seleccione **Crear un certificado**.</span><span class="sxs-lookup"><span data-stu-id="da794-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="da794-112">Seleccione **Elegir archivo**, desplácese hasta el archivo de solicitud de firma de certificado y elija **Cargar**.</span><span class="sxs-lookup"><span data-stu-id="da794-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="da794-113">En la página de confirmación, elija **Descargar** para descargar el archivo de certificado (.pem) y guardar el archivo localmente.</span><span class="sxs-lookup"><span data-stu-id="da794-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="da794-114">**Tenga en cuenta**: el certificado está asociado con el ID. de Apple usado para crearlo.</span><span class="sxs-lookup"><span data-stu-id="da794-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="da794-115">Se recomienda usar un ID de Apple de empresa para las tareas de administración y asegurarse de que el buzón lo supervisa más de una persona o una lista de distribución.</span><span class="sxs-lookup"><span data-stu-id="da794-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="da794-116">Nunca use un ID. de Apple personal.</span><span class="sxs-lookup"><span data-stu-id="da794-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="da794-117">Use el mismo ID. de Apple para renovar el certificado de inserción de Apple cada 12 meses.</span><span class="sxs-lookup"><span data-stu-id="da794-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="da794-118">Escriba el ID. de Apple usado para crear el certificado de inserción de Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="da794-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="da794-119">Registre este identificador como un aviso para cuando necesite renovar el certificado.</span><span class="sxs-lookup"><span data-stu-id="da794-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="da794-120">Vaya al archivo de certificado (.pem), elija **Abrir**y elija **Cargar**.</span><span class="sxs-lookup"><span data-stu-id="da794-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="da794-121">Con el certificado de inserción, Intune puede inscribir y administrar dispositivos Apple.</span><span class="sxs-lookup"><span data-stu-id="da794-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>