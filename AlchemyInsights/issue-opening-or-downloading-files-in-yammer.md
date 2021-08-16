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
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028273"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problema al abrir o descargar archivos en Yammer

La versión clásica de Yammer admite varias opciones de carga de archivos en mensajes y grupos. Según la configuración de la red, los archivos se almacenan de forma predeterminada en SharePoint.

El selector de archivos de la nueva versión de Yammer aún no es compatible con todas las opciones disponibles en la versión clásica de Yammer. En una actualización posterior se agregarán características adicionales. Para obtener más información, vea [Adjuntar un archivo o una imagen a una publicación de conversación de Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**No se puede abrir o descargar un archivo**  

Es posible que un archivo se cargue en Yammer, pero que también esté vinculado a un archivo de SharePoint Online. Para solucionar problemas, en primer lugar debe determinar la ubicación del archivo. Si el archivo se ha cargado en Yammer, tendrá una dirección URL *.yammer.com. Asegúrese de que las direcciones IP y URL necesarias estén desbloqueadas. Para obtener más información, consulte la entrada del blog [No se recomienda el uso de direcciones IP codificadas de forma rígida](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Compruebe si un usuario que también sea administrador global puede descargar el archivo. Si el archivo es privado, puede que tenga que usar el modo de contenido privado. Para obtener más información, vea [Supervisar el contenido privado en Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Archivos e invitados de nivel de red de Yammer en SharePoint Online**  

Los [invitados de nivel de red de Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) no usan B2B de Azure AD y son internos al servicio de Yammer, por lo que no pueden acceder a los archivos de Yammer almacenados en SharePoint. Cree un usuario B2B externo que pueda tener acceso a las bibliotecas de documentos de SharePoint Online con esa identidad. Para obtener más información sobre la futura compatibilidad de invitados de B2B de Azure AD en Yammer, consulte [Soporte para invitados de colaboración entre empresas (B2B) en Yammer (versión preliminar): condiciones para clientes y preguntas más frecuentes](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).