---
title: Ejemplo de directiva contra suplantación de identidad de Microsoft Defender para Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737875"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="f94e5-102">Ejemplo de directiva contra suplantación de identidad de Microsoft Defender para Office 365</span><span class="sxs-lookup"><span data-stu-id="f94e5-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="f94e5-103">Estas opciones de configuración habilitan una directiva denominada *Dominio y CEO.*</span><span class="sxs-lookup"><span data-stu-id="f94e5-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="f94e5-104">Esta directiva proporciona protección de usuario y dominio frente a la suplantación y, a continuación, aplica la directiva a todos los correos electrónicos recibidos por los usuarios del dominio.</span><span class="sxs-lookup"><span data-stu-id="f94e5-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="f94e5-105">En primer lugar, agregue la siguiente información para crear la directiva:</span><span class="sxs-lookup"><span data-stu-id="f94e5-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="f94e5-106">**Nombre:** Descripción del dominio y del director **general:** garantiza que el director ejecutivo y el dominio no se suplanten.</span><span class="sxs-lookup"><span data-stu-id="f94e5-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="f94e5-107">**Se aplica a**: Select **El dominio de destinatario es**.</span><span class="sxs-lookup"><span data-stu-id="f94e5-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="f94e5-108">En **Cualquiera de estos**, seleccione **Elegir** y, a continuación, seleccione un dominio.</span><span class="sxs-lookup"><span data-stu-id="f94e5-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="f94e5-109">Seleccione **+ Agregar**.</span><span class="sxs-lookup"><span data-stu-id="f94e5-109">Select **+ Add**.</span></span> <span data-ttu-id="f94e5-110">Active la casilla situada junto al nombre del dominio de la lista (por ejemplo, *contoso.com*) y, a continuación, **seleccione Agregar**.</span><span class="sxs-lookup"><span data-stu-id="f94e5-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="f94e5-111">Seleccione **Listo**.</span><span class="sxs-lookup"><span data-stu-id="f94e5-111">Select **Done**.</span></span>
- <span data-ttu-id="f94e5-112">Después de crear la directiva, puede ajustarla mediante las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="f94e5-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="f94e5-113">**Agregar usuarios para proteger:** Para este ejemplo, agregue la dirección de correo electrónico del director general, como mínimo.</span><span class="sxs-lookup"><span data-stu-id="f94e5-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="f94e5-114">**Agregar dominios para proteger:** agregue el dominio organizativo que incluye la oficina del director general.</span><span class="sxs-lookup"><span data-stu-id="f94e5-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="f94e5-115">**Choose actions**: For **If email is sent by an suersonated user**, select Redirect message to another email **address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="f94e5-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="f94e5-116">For **If email is sent by an suersonated domain**, select Quarantine the **message**.</span><span class="sxs-lookup"><span data-stu-id="f94e5-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="f94e5-117">**Inteligencia de buzones:** de forma predeterminada, esta opción se selecciona al crear una nueva directiva contra suplantación de identidad.</span><span class="sxs-lookup"><span data-stu-id="f94e5-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="f94e5-118">Deje esta configuración **activada** para obtener mejores resultados.</span><span class="sxs-lookup"><span data-stu-id="f94e5-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="f94e5-119">**Agregar remitentes y dominios de confianza:** En este ejemplo, no defina ninguna invalidación.</span><span class="sxs-lookup"><span data-stu-id="f94e5-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="f94e5-120">Una vez que hayas revisado la configuración, selecciona **Crear esta directiva** o **Guardar**, según corresponda.</span><span class="sxs-lookup"><span data-stu-id="f94e5-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="f94e5-121">Para obtener más información, vea [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="f94e5-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
