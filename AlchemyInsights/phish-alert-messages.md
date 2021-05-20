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
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="67485-102">Alerta de mensajes de correo electrónico de la directiva "Phish Delivered due to tenant or user override".</span><span class="sxs-lookup"><span data-stu-id="67485-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="67485-103">Una directiva de alerta predeterminada denominada "Phish Delivered due to tenant or user override" se ha lanzado a los inquilinos con Microsoft Defender para obtener Office 365 de P1 y P2.</span><span class="sxs-lookup"><span data-stu-id="67485-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="67485-104">Si recibió esta alerta, estos son los pasos para investigar:</span><span class="sxs-lookup"><span data-stu-id="67485-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="67485-105">En el mensaje de alerta, haga clic **en Ver alerta** para ir a la página **Alertas** del Centro de seguridad & cumplimiento.</span><span class="sxs-lookup"><span data-stu-id="67485-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="67485-106">Seleccione la alerta para ver la opción Ver lista **de mensajes** o Ver mensajes en **el Explorador**.</span><span class="sxs-lookup"><span data-stu-id="67485-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="67485-107">Ambas opciones le llevan a los detalles del mensaje, que incluye el id. de mensaje.</span><span class="sxs-lookup"><span data-stu-id="67485-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="67485-108">Tenga en cuenta que el vínculo Explorador de amenazas filtrará automáticamente los mensajes que coinciden con los criterios de alerta.</span><span class="sxs-lookup"><span data-stu-id="67485-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="67485-109">Es posible que deba ajustar el filtro de fecha en el Explorador de amenazas.</span><span class="sxs-lookup"><span data-stu-id="67485-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="67485-110">El mensaje de suplantación de identidad se entregó debido a una invalidación configurada manualmente:</span><span class="sxs-lookup"><span data-stu-id="67485-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="67485-111">Un remitente o dominio permitido establecido por el usuario.</span><span class="sxs-lookup"><span data-stu-id="67485-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="67485-112">Un remitente o dominio permitido establecido por el administrador en una directiva contra correo no deseado.</span><span class="sxs-lookup"><span data-stu-id="67485-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="67485-113">Una dirección IP permitida en una directiva de filtro de conexión.</span><span class="sxs-lookup"><span data-stu-id="67485-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="67485-114">Regla de flujo de correo (también conocida como regla de transporte) que está configurada para permitir la entrada de mensajes.</span><span class="sxs-lookup"><span data-stu-id="67485-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="67485-115">Si cree que el mensaje se marcó incorrectamente como suplantación de identidad, use el complemento Outlook [Report Message para](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) enviar ejemplos de mensajes a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="67485-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
