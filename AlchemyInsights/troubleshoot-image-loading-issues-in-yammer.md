---
title: Solucionar problemas de carga de imagen en Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: 11315fd84f92251e435320f4550286fb2db4b0128f7ac85c0f79972e3f7fd203
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939252"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Solucionar problemas de carga de imagen en Yammer

Cuando se produzcan problemas con las vistas previas de fotos y archivos en Yammer, compruebe si el problema se produce para todos los usuarios, si se produce en dispositivos móviles y si se reproduce al cargar el dato adjunto.  

**Problemas con la foto de perfil**  

Si los usuarios finales inician sesión en Yammer a través de Microsoft 365, deben cambiar su perfil,, incluida la foto de perfil. Si no se permite a los usuarios realizar actualizaciones del perfil, un administrador puede realizar la actualización del usuario. Para obtener más información, consulte [Ver y actualizar el perfil en Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Para obtener más información sobre cómo editar el perfil, incluidas las fotos de perfil, consulte [Cambiar el perfil y la configuración de Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Las fotos de perfil actualizadas se sincronizan de forma diferente que los atributos de perfil. Los usuarios deben iniciar sesión para comenzar una sincronización de la foto de perfil. Para obtener más información, consulte [se actualizan las imágenes de perfil de Office 365 a Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Para obtener más información sobre el ciclo de vida de usuario de Yammer, consulte [Administrar usuarios de Yammer durante su ciclo de vida desde Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Para obtener detalles sobre cómo funciona la sincronización de imágenes de perfil en Microsoft 365, consulte [Información sobre la sincronización de imágenes de perfil en Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Problemas con vistas previas de documentos y vistas en miniatura de imágenes**  

Cuando se publican archivos o imágenes en Yammer, las vistas previas podrían no aparecer debido a lo siguiente: 

- El archivo está dañado y no se puede procesar.
- El archivo no se ha cargado recientemente en SharePoint Online, o Yammer tiene metadatos no válidos por otros motivos.
- Las URL necesarias para cargar las imágenes de vista previa están bloqueadas.
- El usuario ha quitado la vista previa del archivo antes de publicarlo.
- Un problema de servicio impidió que se generara una vista previa.

**Nota** Las vistas previas de vínculos y cargas de archivos pueden tener un comportamiento diferente. Es posible que los vínculos a archivos en Internet o los vínculos que requieren autenticación adicional no se muestren correctamente.

Para obtener más información, consulte [Adjuntar un archivo o una imagen a un mensaje de Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf). 