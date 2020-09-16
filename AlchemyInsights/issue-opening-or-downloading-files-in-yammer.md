---
title: Problema al abrir o descargar archivos en Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695666"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="6b3ca-102">Problema al abrir o descargar archivos en Yammer</span><span class="sxs-lookup"><span data-stu-id="6b3ca-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="6b3ca-103">La versión clásica de Yammer admite varias opciones de carga de archivos en mensajes y grupos.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="6b3ca-104">Según la configuración de la red, los archivos se almacenan de forma predeterminada en SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="6b3ca-105">El selector de archivos de la nueva versión de Yammer aún no es compatible con todas las opciones disponibles en la versión clásica de Yammer.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="6b3ca-106">En una actualización posterior se agregarán características adicionales.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-106">A future update will add additional features.</span></span> <span data-ttu-id="6b3ca-107">Para obtener más información, vea [Adjuntar un archivo o una imagen a una publicación de conversación de Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="6b3ca-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="6b3ca-108">**No se puede abrir o descargar un archivo**</span><span class="sxs-lookup"><span data-stu-id="6b3ca-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="6b3ca-109">Es posible que un archivo se cargue en Yammer, pero que también esté vinculado a un archivo de SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="6b3ca-110">Para solucionar problemas, en primer lugar debe determinar la ubicación del archivo.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="6b3ca-111">Si el archivo se ha cargado en Yammer, tendrá una dirección URL \*.yammer.com.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="6b3ca-112">Asegúrese de que las direcciones IP y URL necesarias estén desbloqueadas.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="6b3ca-113">Para obtener más información, consulte la entrada del blog [No se recomienda el uso de direcciones IP codificadas de forma rígida](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="6b3ca-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="6b3ca-114">Compruebe si un usuario que también sea administrador global puede descargar el archivo.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="6b3ca-115">Si el archivo es privado, puede que tenga que usar el modo de contenido privado.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="6b3ca-116">Para obtener más información, vea [Supervisar el contenido privado en Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="6b3ca-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="6b3ca-117">**Archivos e invitados de nivel de red de Yammer en SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="6b3ca-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="6b3ca-118">Los [invitados de nivel de red de Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) no usan B2B de Azure AD y son internos al servicio de Yammer, por lo que no pueden acceder a los archivos de Yammer almacenados en SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="6b3ca-119">Cree un usuario B2B externo que pueda tener acceso a las bibliotecas de documentos de SharePoint Online con esa identidad.</span><span class="sxs-lookup"><span data-stu-id="6b3ca-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="6b3ca-120">Para obtener más información sobre la futura compatibilidad de invitados de B2B de Azure AD en Yammer, consulte [Soporte para invitados de colaboración entre empresas (B2B) en Yammer (versión preliminar): condiciones para clientes y preguntas más frecuentes](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="6b3ca-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>