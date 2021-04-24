---
title: Directivas de retención en el Centro de administración de Exchange que no funcionan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952245"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="e0274-102">Directivas de retención en el Centro de administración de Exchange</span><span class="sxs-lookup"><span data-stu-id="e0274-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="e0274-103">Si desea que ejecutemos comprobaciones automatizadas para la configuración mencionada a continuación, seleccione el botón atrás <-- en la parte superior de esta página y, a continuación, escriba la dirección de correo electrónico del usuario que tiene problemas con las directivas de retención.</span><span class="sxs-lookup"><span data-stu-id="e0274-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="e0274-104">Si tiene problemas con las directivas de retención en el Centro de administración de Exchange que no se aplican a buzones o elementos que no se mueven al buzón de archivo, compruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="e0274-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="e0274-105">**Causas raíz:**</span><span class="sxs-lookup"><span data-stu-id="e0274-105">**Root Causes:**</span></span>

- <span data-ttu-id="e0274-106">**El Asistente para carpetas** administradas no ha procesado el buzón del usuario.</span><span class="sxs-lookup"><span data-stu-id="e0274-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="e0274-107">El Asistente para carpetas administradas intenta procesar todos los buzones de la organización basada en la nube una vez cada siete días.</span><span class="sxs-lookup"><span data-stu-id="e0274-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="e0274-108">**Solución:** Ejecute el Asistente para carpeta administrada.</span><span class="sxs-lookup"><span data-stu-id="e0274-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="e0274-109">**RetentionHold** se ha **habilitado** en el buzón.</span><span class="sxs-lookup"><span data-stu-id="e0274-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="e0274-110">Si el buzón se ha colocado en retentionHold, la directiva de retención en el buzón no se procesará durante ese tiempo.</span><span class="sxs-lookup"><span data-stu-id="e0274-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="e0274-111">**Solución:** Compruebe el estado de la configuración de retención y actualice según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="e0274-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="e0274-112">Para obtener más información, vea [Retención de buzones de correo.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="e0274-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="e0274-113">**Nota:** Si un buzón es menor que 10 MB, el Asistente para carpetas administradas no procesará automáticamente el buzón.</span><span class="sxs-lookup"><span data-stu-id="e0274-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="e0274-114">Para obtener más información sobre las directivas de retención en el Centro de administración de Exchange, vea:</span><span class="sxs-lookup"><span data-stu-id="e0274-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="e0274-115">Etiquetas de retención y directivas de retención</span><span class="sxs-lookup"><span data-stu-id="e0274-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="e0274-116">[Aplicar una directiva de retención a buzones o](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Agregar o quitar etiquetas de retención](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="e0274-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="e0274-117">Cómo identificar el tipo de retención en un buzón</span><span class="sxs-lookup"><span data-stu-id="e0274-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
