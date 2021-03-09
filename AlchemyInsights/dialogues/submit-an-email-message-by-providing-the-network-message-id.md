---
title: Enviar un mensaje de correo electrónico proporcionando el id. de mensaje de red
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552480"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="44868-102">Enviar un mensaje de correo electrónico proporcionando el id. de mensaje de red</span><span class="sxs-lookup"><span data-stu-id="44868-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="44868-103">En el **menú desplegable** Nuevo envío, seleccione **Correo** electrónico e **Id. de mensaje de red.**</span><span class="sxs-lookup"><span data-stu-id="44868-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="44868-104">Siga estos pasos para buscar el identificador de mensaje de un mensaje de correo electrónico en Outlook:</span><span class="sxs-lookup"><span data-stu-id="44868-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="44868-105">Haga doble clic en el mensaje de correo electrónico para abrirlo.</span><span class="sxs-lookup"><span data-stu-id="44868-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="44868-106">Seleccione **Propiedades del**  >  **archivo**.</span><span class="sxs-lookup"><span data-stu-id="44868-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="44868-107">Abra el Bloc de notas o un documento de Word en blanco y, a continuación, copie y pegue el contenido encontrado en el cuadro Encabezados de **Internet** en el documento abierto para obtener una mejor visibilidad.</span><span class="sxs-lookup"><span data-stu-id="44868-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="44868-108">Busque el **campo X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="44868-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="44868-109">El valor después de **:** es el identificador que necesita para el envío.</span><span class="sxs-lookup"><span data-stu-id="44868-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="44868-110">En **Destinatarios**, si el correo electrónico aterrizó en la carpeta de correo no deseado para todos los destinatarios de este correo electrónico, elija **Seleccionar todo**.</span><span class="sxs-lookup"><span data-stu-id="44868-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="44868-111">Si no es así, seleccione solo el usuario que ha notificado el problema.</span><span class="sxs-lookup"><span data-stu-id="44868-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="44868-112">En **Motivo del** envío , si selecciona Debería haber sido bloqueado , especifique si el mensaje debe haber sido bloqueado como **Correo** no deseado, **Suplantación** de identidad o **Malware** y, a continuación, **seleccione Enviar**. </span><span class="sxs-lookup"><span data-stu-id="44868-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="44868-113">Para obtener más información, vea [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="44868-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
