---
title: Archivo de solo lectura abierto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813201"
---
# <a name="file-open-read-only"></a><span data-ttu-id="e3b7c-102">Archivo de solo lectura abierto</span><span class="sxs-lookup"><span data-stu-id="e3b7c-102">File open read-only</span></span>

<span data-ttu-id="e3b7c-103">Puede que encuentre que al abrir archivos, se abren como de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="e3b7c-104">En algunos casos, esto es para mayor seguridad, como cuando se abren archivos desde Internet y otras veces, puede deberse a una configuración que se puede cambiar.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="e3b7c-105">Estos son algunos escenarios en los que un archivo abre de solo lectura y algunos pasos que puede seguir para cambiarlo.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="e3b7c-106">**Mi antivirus hace que abran solo lectura**</span><span class="sxs-lookup"><span data-stu-id="e3b7c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="e3b7c-107">Algunos programas antivirus pueden protegerle de archivos potencialmente no seguros al abrirlos de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="e3b7c-108">Es posible que deba consultar con su proveedor de antivirus para obtener información sobre cómo ajustar esta configuración.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="e3b7c-109">BitDefender, por ejemplo, tiene contenido sobre cómo agregar exclusiones de aplicaciones aquí: Cómo agregar exclusiones de aplicaciones o procesos en el Centro de [control de Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="e3b7c-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="e3b7c-110">**¿Las propiedades del archivo están establecidas en solo lectura?**</span><span class="sxs-lookup"><span data-stu-id="e3b7c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="e3b7c-111">Para comprobar las propiedades del archivo, haga clic con el botón secundario en el archivo y elija Propiedades.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="e3b7c-112">Si el atributo de solo lectura está activado, puede desactivarlo y hacer clic en Aceptar.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="e3b7c-113">**El contenido está en la vista protegida**</span><span class="sxs-lookup"><span data-stu-id="e3b7c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="e3b7c-114">Los archivos de Internet y de otras ubicaciones potencialmente no seguras pueden contener virus, gusanos u otros tipos de malware que pueden dañar el equipo.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="e3b7c-115">Esto también es habitual con los datos adjuntos de correo electrónico o los archivos que has descargado.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="e3b7c-116">Para ayudar a proteger el equipo, los archivos de estas ubicaciones potencialmente no seguras se abren en la vista protegida.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="e3b7c-117">Al usar la vista protegida, puede leer un archivo y ver su contenido al mismo tiempo que reduce los riesgos.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="e3b7c-118">Para obtener más información sobre la vista protegida y cómo cambiar la configuración, vea este artículo: [¿Qué es la vista protegida?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="e3b7c-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="e3b7c-119">**¿OneDrive está lleno?**</span><span class="sxs-lookup"><span data-stu-id="e3b7c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="e3b7c-120">Si el archivo se almacena en OneDrive y el espacio de almacenamiento de OneDrive está lleno, no podrá guardar el documento hasta que esté bajo el espacio asignado.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="e3b7c-121">Puede comprobar el espacio libre en OneDrive haciendo clic en el icono de OneDrive en el centro de notificaciones y eligiendo Administrar almacenamiento, o puede ir a , iniciar sesión y tener en cuenta la cantidad de espacio usado en la parte inferior izquierda de la [https://onedrive.live.com](https://onedrive.live.com) pantalla.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="e3b7c-122">**¿Office está activado?**</span><span class="sxs-lookup"><span data-stu-id="e3b7c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="e3b7c-123">Si Office no está activado o si la suscripción ha expirado, podría estar en modo de funcionalidad reducida de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="e3b7c-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="e3b7c-124">Para obtener información sobre cómo activar Office, vea: Errores de activación y producto sin [licencia en Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="e3b7c-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="e3b7c-125">**Si todo lo demás falla...**</span><span class="sxs-lookup"><span data-stu-id="e3b7c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="e3b7c-126">Intente reiniciar el equipo</span><span class="sxs-lookup"><span data-stu-id="e3b7c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="e3b7c-127">Instalar actualizaciones de Office</span><span class="sxs-lookup"><span data-stu-id="e3b7c-127">Install Office updates</span></span>
    
- <span data-ttu-id="e3b7c-128">Realizar una reparación en línea de Office</span><span class="sxs-lookup"><span data-stu-id="e3b7c-128">Perform an Online repair of Office</span></span>
    

