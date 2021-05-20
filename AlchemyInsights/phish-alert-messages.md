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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544595"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alerta de mensajes de correo electrónico de la directiva "Phish Delivered due to tenant or user override".

Una directiva de alerta predeterminada denominada "Phish Delivered due to tenant or user override" se ha lanzado a los inquilinos con Microsoft Defender para obtener Office 365 de P1 y P2. Si recibió esta alerta, estos son los pasos para investigar:

1. En el mensaje de alerta, haga clic **en Ver alerta** para ir a la página **Alertas** del Centro de seguridad & cumplimiento.

2. Seleccione la alerta para ver la opción Ver lista **de mensajes** o Ver mensajes en **el Explorador**. Ambas opciones le llevan a los detalles del mensaje, que incluye el id. de mensaje. Tenga en cuenta que el vínculo Explorador de amenazas filtrará automáticamente los mensajes que coinciden con los criterios de alerta. Es posible que deba ajustar el filtro de fecha en el Explorador de amenazas.

El mensaje de suplantación de identidad se entregó debido a una invalidación configurada manualmente:

- Un remitente o dominio permitido establecido por el usuario.

- Un remitente o dominio permitido establecido por el administrador en una directiva contra correo no deseado.

- Una dirección IP permitida en una directiva de filtro de conexión.

- Regla de flujo de correo (también conocida como regla de transporte) que está configurada para permitir la entrada de mensajes.

Si cree que el mensaje se marcó incorrectamente como suplantación de identidad, use el complemento Outlook [Report Message para](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) enviar ejemplos de mensajes a Microsoft.
