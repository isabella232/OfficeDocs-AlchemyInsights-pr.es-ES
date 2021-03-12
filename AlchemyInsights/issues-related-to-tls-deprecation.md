---
title: No se puede enviar o recibir correo electrónico desde Office 365 debido a la deshabilitación de TLS 1.0 y TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726936"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="09ed7-102">No se puede enviar o recibir correo electrónico desde Office 365 debido a la deshabilitación de TLS 1.0 y TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="09ed7-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="09ed7-103">Como confirma la publicación del centro de mensajes MC229914, la desuso de TLS 1.0 y TLS 1.1 comenzó a aplicar para los extremos de flujo de correo de Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="09ed7-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="09ed7-104">Pronto Office 365 ya no aceptará conexiones de correo electrónico TLS 1.0 y TLS 1.1 desde orígenes externos.</span><span class="sxs-lookup"><span data-stu-id="09ed7-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="09ed7-105">Además, Exchange Online nunca usará TLS 1.0 o 1.1 para enviar correo electrónico saliente.</span><span class="sxs-lookup"><span data-stu-id="09ed7-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="09ed7-106">Si tiene problemas debido a la deshabilitación de TLS 1.0 o 1.1, es posible que experimente uno de los siguientes errores:</span><span class="sxs-lookup"><span data-stu-id="09ed7-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="09ed7-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="09ed7-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="09ed7-108">Error en el Visor de cola del servidor local que envía correo electrónico al oficial 365- '421 4.4.2 Conexión descartada debido a SocketError'</span><span class="sxs-lookup"><span data-stu-id="09ed7-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="09ed7-109">Error en el registro de protocolo del [conector de envío](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) en el servidor que envía correo electrónico a Office 365: error al negociar TLS con el error SocketError</span><span class="sxs-lookup"><span data-stu-id="09ed7-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="09ed7-110">Error en el registro de protocolo del conector de envío o recepción: '451 5.7.3 Debe emitir primero un comando STARTTLS'</span><span class="sxs-lookup"><span data-stu-id="09ed7-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="09ed7-111">Si experimenta alguno de los errores anteriores, asegúrese de que el servidor que envía o recibe correo electrónico tiene TLS 1.2 habilitado comprobando las siguientes claves del Registro-</span><span class="sxs-lookup"><span data-stu-id="09ed7-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="09ed7-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="09ed7-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="09ed7-113">Si realiza algún cambio en las claves del Registro anteriores para habilitar TLS 1.2, reinicie el servidor para que los cambios entren en vigor.</span><span class="sxs-lookup"><span data-stu-id="09ed7-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="09ed7-114">Asegúrese también de tener instaladas las actualizaciones más recientes de Windows y Exchange.</span><span class="sxs-lookup"><span data-stu-id="09ed7-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="09ed7-115">Para obtener más información, vea:</span><span class="sxs-lookup"><span data-stu-id="09ed7-115">For more information, see:</span></span>

- [<span data-ttu-id="09ed7-116">Exchange Server de TLS, parte 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="09ed7-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="09ed7-117">Exchange Server de TLS parte 2: Habilitar TLS 1.2 e Identificar clientes que no lo usan: Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="09ed7-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="09ed7-118">Descripción de los escenarios de correo electrónico si las versiones tls no se pueden acordar con Exchange Online- Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="09ed7-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
