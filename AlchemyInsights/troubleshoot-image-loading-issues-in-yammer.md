---
title: Solucionar problemas de carga de imagen en Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146805"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="fc5d3-102">Solucionar problemas de carga de imagen en Yammer</span><span class="sxs-lookup"><span data-stu-id="fc5d3-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="fc5d3-103">Cuando se produzcan problemas con las vistas previas de fotos y archivos en Yammer, compruebe si el problema se produce para todos los usuarios, si se produce en dispositivos móviles y si se reproduce al cargar el dato adjunto.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="fc5d3-104">**Problemas con la foto de perfil**</span><span class="sxs-lookup"><span data-stu-id="fc5d3-104">**Profile photo issues**</span></span>  

<span data-ttu-id="fc5d3-105">Si los usuarios finales inician sesión en Yammer a través de Microsoft 365, deben cambiar su perfil,, incluida la foto de perfil.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="fc5d3-106">Si no se permite a los usuarios realizar actualizaciones del perfil, un administrador puede realizar la actualización del usuario.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="fc5d3-107">Para obtener más información, consulte [Ver y actualizar el perfil en Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="fc5d3-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="fc5d3-108">Para obtener más información sobre cómo editar el perfil, incluidas las fotos de perfil, consulte [Cambiar el perfil y la configuración de Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="fc5d3-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="fc5d3-109">Las fotos de perfil actualizadas se sincronizan de forma diferente que los atributos de perfil.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="fc5d3-110">Los usuarios deben iniciar sesión para comenzar una sincronización de la foto de perfil.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="fc5d3-111">Para obtener más información, consulte [se actualizan las imágenes de perfil de Office 365 a Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="fc5d3-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="fc5d3-112">Para obtener más información sobre el ciclo de vida de usuario de Yammer, consulte [Administrar usuarios de Yammer durante su ciclo de vida desde Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="fc5d3-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="fc5d3-113">Para obtener detalles sobre cómo funciona la sincronización de imágenes de perfil en Microsoft 365, consulte [Información sobre la sincronización de imágenes de perfil en Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="fc5d3-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="fc5d3-114">**Problemas con vistas previas de documentos y vistas en miniatura de imágenes**</span><span class="sxs-lookup"><span data-stu-id="fc5d3-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="fc5d3-115">Cuando se publican archivos o imágenes en Yammer, las vistas previas podrían no aparecer debido a lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="fc5d3-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="fc5d3-116">El archivo está dañado y no se puede procesar.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="fc5d3-117">El archivo no se ha cargado recientemente en SharePoint Online, o Yammer tiene metadatos no válidos por otros motivos.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="fc5d3-118">Las URL necesarias para cargar las imágenes de vista previa están bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="fc5d3-119">El usuario ha quitado la vista previa del archivo antes de publicarlo.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="fc5d3-120">Un problema de servicio impidió que se generara una vista previa.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="fc5d3-121">**Nota** Las vistas previas de vínculos y cargas de archivos pueden tener un comportamiento diferente.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="fc5d3-122">Es posible que los vínculos a archivos en Internet o los vínculos que requieren autenticación adicional no se muestren correctamente.</span><span class="sxs-lookup"><span data-stu-id="fc5d3-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="fc5d3-123">Para obtener más información, consulte [Adjuntar un archivo o una imagen a un mensaje de Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="fc5d3-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 