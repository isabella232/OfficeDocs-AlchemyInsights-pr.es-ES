---
title: 2681 Attack Simulator en Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545743"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="27613-102">Simulador de ataque en Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="27613-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="27613-103">¿Falta el simulador de ataque?</span><span class="sxs-lookup"><span data-stu-id="27613-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="27613-104">Attack Simulator requiere **Microsoft Defender para Office 365 plan 2** o Office 365 Enterprise **E5**.</span><span class="sxs-lookup"><span data-stu-id="27613-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="27613-105">Attack Simulator no **se incluye** en Microsoft Defender para Office 365 plan 1, Office 365 Enterprise E3 ni ninguna Aplicaciones Microsoft 365 para negocios suscripciones.</span><span class="sxs-lookup"><span data-stu-id="27613-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="27613-106">La cuenta que use para iniciar ataques simulados requiere permisos de administrador global o de administrador de seguridad y autenticación multifactor (MFA).</span><span class="sxs-lookup"><span data-stu-id="27613-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="27613-107">Para obtener más información acerca de los requisitos de Attack Simulator, vea [este tema](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="27613-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="27613-108">Aspectos importantes que debe saber acerca de las simulaciones **de ataque** de contraseña de fuerza bruta:</span><span class="sxs-lookup"><span data-stu-id="27613-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="27613-109">Si la cuenta de destino tiene MFA habilitada y la contraseña se ha adivinado correctamente, la cuenta no se mostrará como comprometida (el segundo factor de autenticación estará incompleto).</span><span class="sxs-lookup"><span data-stu-id="27613-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="27613-110">El archivo de contraseña no puede tener más de 10 MB.</span><span class="sxs-lookup"><span data-stu-id="27613-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="27613-111">Use una contraseña por línea e incluya una línea en blanco (retorno de carro) después de la última contraseña de la lista.</span><span class="sxs-lookup"><span data-stu-id="27613-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="27613-112">Aspectos importantes que debe saber acerca de las simulaciones **de conexión de phishing** de Lanza:</span><span class="sxs-lookup"><span data-stu-id="27613-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="27613-113">Por diseño, no puede proporcionar un valor personalizado para la dirección URL del servidor de inicio de **sesión de phishing**.</span><span class="sxs-lookup"><span data-stu-id="27613-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="27613-114">Si un destinatario [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) usa el complemento Habilitar el mensaje de informe para notificar el mensaje como suplantación de identidad, es posible que no reciba alertas para el mensaje (porque se trata de un ataque simulado).</span><span class="sxs-lookup"><span data-stu-id="27613-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="27613-115">Informes: una vez completado el ataque simulado, puedes hacer clic en **Detalles de ataque** para ver el informe.</span><span class="sxs-lookup"><span data-stu-id="27613-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="27613-116">Para obtener instrucciones detalladas y nuevas características en Attack Simulator, consulta [Attack Simulator en Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="27613-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
