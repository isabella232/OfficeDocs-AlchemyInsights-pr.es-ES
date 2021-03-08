---
title: Registros de contraseñas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523093"
---
# <a name="password-logs"></a><span data-ttu-id="22cd1-102">Registros de contraseñas</span><span class="sxs-lookup"><span data-stu-id="22cd1-102">Password logs</span></span>

<span data-ttu-id="22cd1-103">**Tengo problemas al acceder a los registros de auditoría del restablecimiento de contraseña**</span><span class="sxs-lookup"><span data-stu-id="22cd1-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="22cd1-104">Para solucionar los problemas relacionados con el acceso a los registros de auditoría del restablecimiento de contraseña, realice el siguiente paso:</span><span class="sxs-lookup"><span data-stu-id="22cd1-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="22cd1-105">Asegúrese de que está autorizado para ver los registros de auditoría.</span><span class="sxs-lookup"><span data-stu-id="22cd1-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="22cd1-106">Solo se autorizan los roles siguientes:</span><span class="sxs-lookup"><span data-stu-id="22cd1-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="22cd1-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="22cd1-107">Global administrator</span></span>
 - <span data-ttu-id="22cd1-108">Administrador de seguridad</span><span class="sxs-lookup"><span data-stu-id="22cd1-108">Security administrator</span></span>
 - <span data-ttu-id="22cd1-109">Lector de seguridad</span><span class="sxs-lookup"><span data-stu-id="22cd1-109">Security reader</span></span>

<span data-ttu-id="22cd1-110">**Quiero ver todos los eventos de auditoría del restablecimiento de contraseñas desde el momento de la implementación inicial**</span><span class="sxs-lookup"><span data-stu-id="22cd1-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="22cd1-111">Se almacenan hasta 120 000 eventos de restablecimiento o registro de contraseñas en los informes de los últimos 30 días.</span><span class="sxs-lookup"><span data-stu-id="22cd1-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="22cd1-112">Este límite máximo se aplica a la interfaz de usuario al descargar el archivo CSV.</span><span class="sxs-lookup"><span data-stu-id="22cd1-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="22cd1-113">Hay disponibles 1 millón de eventos a través de PowerShell.</span><span class="sxs-lookup"><span data-stu-id="22cd1-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="22cd1-114">Para más información, vea los vínculos siguientes:</span><span class="sxs-lookup"><span data-stu-id="22cd1-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="22cd1-115">Eventos de restablecimiento de contraseña de autoservicio desde Azure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="22cd1-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="22cd1-116">Cómo descargar rápidamente eventos de registro de restablecimiento de contraseña con PowerShell</span><span class="sxs-lookup"><span data-stu-id="22cd1-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="22cd1-117">**Quiero obtener más información sobre las funcionalidades de informes de restablecimiento de contraseñas**</span><span class="sxs-lookup"><span data-stu-id="22cd1-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="22cd1-118">Compruebe quién se registra o restablece contraseñas con los registros de auditoría de restablecimiento de contraseña de Azure AD en Azure Portal en **Usuarios y grupos**.</span><span class="sxs-lookup"><span data-stu-id="22cd1-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="22cd1-119">Para más información, consulte los siguientes vínculos:</span><span class="sxs-lookup"><span data-stu-id="22cd1-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="22cd1-120">Información general sobre los informes de restablecimiento de contraseña</span><span class="sxs-lookup"><span data-stu-id="22cd1-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="22cd1-121">Cómo ver los informes de restablecimiento de contraseña en Azure Portal</span><span class="sxs-lookup"><span data-stu-id="22cd1-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="22cd1-122">Eventos de restablecimiento de contraseña de autoservicio desde Azure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="22cd1-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="22cd1-123">Cómo descargar rápidamente eventos de registro de restablecimiento de contraseña con PowerShell</span><span class="sxs-lookup"><span data-stu-id="22cd1-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


