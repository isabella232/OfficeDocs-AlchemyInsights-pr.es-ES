---
title: Sesiones activas múltiples en el mismo buzón
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
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769740"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="ef56c-102">Sesiones activas múltiples en el mismo buzón</span><span class="sxs-lookup"><span data-stu-id="ef56c-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="ef56c-103">Para controlar el uso de los recursos de Exchange, un buzón de correo tiene un "presupuesto".</span><span class="sxs-lookup"><span data-stu-id="ef56c-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="ef56c-104">La excepción de presupuesto excedido se puede desencadenar, aunque no solamente, por las siguientes circunstancias:</span><span class="sxs-lookup"><span data-stu-id="ef56c-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="ef56c-105">Algunas pestañas del explorador están abiertas en la misma sesión de Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ef56c-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="ef56c-106">Algunas sesiones de Outlook Web App están activas para el mismo buzón de correo.</span><span class="sxs-lookup"><span data-stu-id="ef56c-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="ef56c-107">Otras aplicaciones de cliente (Outlook, Outlook Mobile, una aplicación cliente de terceros) tienen acceso al buzón de correo al mismo tiempo.</span><span class="sxs-lookup"><span data-stu-id="ef56c-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="ef56c-108">Las operaciones prolongadas, como ejecutar solicitudes de búsqueda, se llevan a cabo en otra sesión de buzón activo.</span><span class="sxs-lookup"><span data-stu-id="ef56c-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

