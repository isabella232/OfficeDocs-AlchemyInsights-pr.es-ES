---
title: Varios objetos tienen la misma dirección de correo electrónico que la identidad
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
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724632"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="b78b4-102">Varios objetos tienen la misma dirección de correo electrónico que la identidad</span><span class="sxs-lookup"><span data-stu-id="b78b4-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="b78b4-103">**Varios objetos**</span><span class="sxs-lookup"><span data-stu-id="b78b4-103">**Multiple objects**</span></span>

<span data-ttu-id="b78b4-104">Uno de los motivos comunes de este error es que no pueda redirigir correctamente una solicitud de Outlook Web Access en la presencia de varios objetos que tengan la misma dirección de correo electrónico que la identidad.</span><span class="sxs-lookup"><span data-stu-id="b78b4-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="b78b4-105">Para encontrar estos objetos, ejecute los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="b78b4-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="b78b4-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="b78b4-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="b78b4-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="b78b4-107">· Get-User <email address></span></span>

<span data-ttu-id="b78b4-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="b78b4-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="b78b4-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="b78b4-109">· Get-Contact <email address></span></span>

<span data-ttu-id="b78b4-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="b78b4-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="b78b4-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="b78b4-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="b78b4-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="b78b4-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="b78b4-113">Para resolver este problema, quite varios objetos con la misma identidad de correo electrónico y asegúrese de que existe un único objeto con la identidad de correo electrónico específica y de que su tipo de destinatario es UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="b78b4-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="b78b4-114">**La misma dirección se usa para los buzones de cliente y empresa**</span><span class="sxs-lookup"><span data-stu-id="b78b4-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="b78b4-115">Otra causa es cuando se usa la misma dirección para los buzones de cliente y de empresa.</span><span class="sxs-lookup"><span data-stu-id="b78b4-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="b78b4-116">En este caso, el usuario tendrá que cambiar el alias de consumidor principal hasta que cibercafé sea compatible con este escenario.</span><span class="sxs-lookup"><span data-stu-id="b78b4-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="b78b4-117">Este es un error permanente que no desaparecerá sin intervención.</span><span class="sxs-lookup"><span data-stu-id="b78b4-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="b78b4-118">Para obtener más información, consulte [Cambiar la dirección de correo electrónico o el número de teléfono de la cuenta de Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="b78b4-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>