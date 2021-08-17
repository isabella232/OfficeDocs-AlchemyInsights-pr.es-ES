---
title: No se puede enviar o recibir correo electrónico Office 365 debido a la deshabilitación tls 1.0 y TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054923"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>No se puede enviar o recibir correo electrónico Office 365 debido a la deshabilitación tls 1.0 y TLS 1.1

Tal como lo confirma la publicación del centro de mensajes MC229914, la desusación de TLS 1.0 y TLS 1.1 comenzó a aplicar para Exchange Online de flujo de correo. Pronto Office 365 aceptará conexiones de correo electrónico TLS 1.0 y TLS 1.1 desde orígenes externos. Además, Exchange Online usará TLS 1.0 o 1.1 para enviar correo electrónico saliente. Si tiene problemas debido a la deshabilitación de TLS 1.0 o 1.1, es posible que experimente uno de los siguientes errores:

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Error en el Visor de cola del servidor local que envía correo electrónico al oficial 365- '421 4.4.2 Conexión descartada debido a SocketError'
- Error en el registro de protocolo del [conector de envío](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) en el servidor que envía correo electrónico a Office 365- Error en la negociación TLS con el error SocketError
- Error en el registro de protocolo del conector de envío o recepción: '451 5.7.3 Debe emitir primero un comando STARTTLS'

Si experimenta alguno de los errores anteriores, asegúrese de que el servidor que envía o recibe correo electrónico tiene TLS 1.2 habilitado comprobando las siguientes claves del Registro-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Si realiza algún cambio en las claves del Registro anteriores para habilitar TLS 1.2, reinicie el servidor para que los cambios entren en vigor. Asegúrese también de que tiene las actualizaciones Windows y Exchange instaladas.

Para obtener más información, vea:

- [Exchange Server Instrucciones tls, parte 1: Prepararse para TLS 1.2: Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Instrucciones tls Parte 2: Habilitar TLS 1.2 e Identificar clientes que no lo usan: Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Descripción de los escenarios de correo electrónico si las versiones tls no se pueden acordar con Exchange Online: Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
