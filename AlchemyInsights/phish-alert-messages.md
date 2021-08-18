---
title: 2491 Alerta de mensajes de correo electrónico de la directiva "Phish Delivered due to tenant or user override"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316375"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alerta de mensajes de correo electrónico de la directiva "Phish Delivered due to tenant or user override".

Una directiva de alerta predeterminada denominada **Phish Delivered debido** a la invalidación de inquilino o usuario está disponible en organizaciones con Microsoft Defender para Office 365 licencias P1 y P2. Si recibió esta alerta, estos son los pasos para investigar:

1. En el mensaje de alerta, haga clic **en Ver alerta** para ir a la página **Alertas** del portal de Microsoft 365 Defender alertas.

2. Seleccione la alerta para ver la opción Ver lista **de mensajes** o Ver mensajes en **el Explorador**. Ambas opciones le llevan a los detalles del mensaje, que incluye el id. de mensaje. Tenga en cuenta que el vínculo Explorador de amenazas filtrará automáticamente los mensajes que coinciden con los criterios de alerta. Es posible que deba ajustar el filtro de fecha en el Explorador de amenazas.

El mensaje de suplantación de identidad se entregó debido a una invalidación configurada manualmente:

- Un remitente o dominio permitido establecido por el usuario.
- Un remitente o dominio permitido establecido por el administrador en una directiva contra correo no deseado.
- Una dirección IP permitida en una directiva de filtro de conexión.
- Regla de flujo de correo (también conocida como regla de transporte) que está configurada para permitir la entrada de mensajes.

Si cree que el mensaje se marcó incorrectamente como suplantación de identidad, use el envío [de](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) administrador para notificar el mensaje a Microsoft.

Los usuarios pueden usar el complemento Report Message o el complemento [Report Phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) en Outlook enviar ejemplos de mensajes a Microsoft.
