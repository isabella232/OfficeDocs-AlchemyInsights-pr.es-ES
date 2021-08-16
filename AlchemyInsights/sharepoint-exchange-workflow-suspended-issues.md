---
title: Introducción a SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: a14705003f742641f10c8459b7c7024146e4134a8d5113451e5732cef7326484
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54051431"
---
# <a name="workflows-in-sharepoint"></a>Flujos de trabajo de SharePoint

Si SharePoint flujos de trabajo no envían correos electrónicos, es posible que su organización haya encontrado los límites Exchange Online remitente.

Puede producirse el mensaje de error "Flujo de trabajo suspendido" si tiene uno de los siguientes elementos:

- Tiene un flujo de trabajo en SharePoint Online que usa el tipo de plataforma de flujo de trabajo SharePoint 2010 SharePoint 2013.

- El flujo de trabajo está configurado para enviar un mensaje de correo electrónico personalizado a más de 200 usuarios a la vez, más de 10 000 destinatarios al día o más de 30 mensajes por minuto.

Al ejecutar el flujo de trabajo, el mensaje de correo electrónico no se envía y observa el mensaje de error, El estado interno se establece en Suspendido o No se puede enviar a un destinatario.

Para obtener más información, consulte el siguiente [artículo](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

