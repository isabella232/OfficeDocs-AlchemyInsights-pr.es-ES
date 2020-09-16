---
title: Eliminar un canal privado de Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730932"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="3276b-102">Eliminar un canal privado de Teams</span><span class="sxs-lookup"><span data-stu-id="3276b-102">Delete a Teams private channel</span></span>

<span data-ttu-id="3276b-103">Microsoft es consciente de un problema al eliminar un canal privado de Teams si tiene habilitadas las directivas de retención de SharePoint para el sitio de SharePoint subyacente.</span><span class="sxs-lookup"><span data-stu-id="3276b-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="3276b-104">Microsoft está trabajando para solucionar este problema.</span><span class="sxs-lookup"><span data-stu-id="3276b-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="3276b-105">Mientras tanto, puede usar una de las siguientes soluciones alternativas para eliminar dicho canal privado.</span><span class="sxs-lookup"><span data-stu-id="3276b-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="3276b-106">**Excluya la colección equipo/sitio de la directiva de retención de SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="3276b-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="3276b-107">Diríjase al portal de administración de Office 365 y seleccione **Mostrar todo** en el panel de navegación izquierdo.</span><span class="sxs-lookup"><span data-stu-id="3276b-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="3276b-108">En **Centros de administración**, diríjase a **Seguridad y cumplimiento** > **Prevención de pérdida de datos** > **Directiva**.</span><span class="sxs-lookup"><span data-stu-id="3276b-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="3276b-109">Identifique cualquier directiva que se aplique a los sitios de SharePoint y modifíquela, de manera que el sitio de SharePoint para el equipo que contiene el canal privado NO se incluya en la directiva de retención.</span><span class="sxs-lookup"><span data-stu-id="3276b-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="3276b-110">Guarde la directiva.</span><span class="sxs-lookup"><span data-stu-id="3276b-110">Save the policy.</span></span>
    <span data-ttu-id="3276b-111">Las configuraciones de directivas pueden tardar hasta 24 horas en tener efecto.</span><span class="sxs-lookup"><span data-stu-id="3276b-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="3276b-112">Después de que se haya excluido el sitio, puede eliminar el canal privado.</span><span class="sxs-lookup"><span data-stu-id="3276b-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="3276b-113">Es ***posible*** que pueda eliminar el canal privado desde Microsoft Teams en su dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="3276b-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="3276b-114">Para obtener información relacionada con SharePoint, consulte [No se pueden eliminar elementos en SharePoint Online o OneDrive para la Empresa](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="3276b-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>