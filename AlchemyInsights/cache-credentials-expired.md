---
title: 'Error: no se pueden cargar ni descargar los cambios porque han expirado las credenciales almacenadas en caché'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734496"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a><span data-ttu-id="fe801-102">Error: no se pueden cargar ni descargar los cambios porque han expirado las credenciales almacenadas en caché</span><span class="sxs-lookup"><span data-stu-id="fe801-102">Error: We can't upload or download your changes because your cached credentials have expired</span></span>

<span data-ttu-id="fe801-103">Al guardar archivos en la aplicación de OneDrive, si recibe un error que contiene la frase **"sus credenciales almacenadas en caché han expirado"**, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="fe801-103">When saving files to the OneDrive app, if you receive an error that contains the phrase **"your cached credentials have expired"**, perform the following steps:</span></span>

1. <span data-ttu-id="fe801-104">Cierre todas las aplicaciones de Office.</span><span class="sxs-lookup"><span data-stu-id="fe801-104">Close all Office applications.</span></span>
1. <span data-ttu-id="fe801-105">Abra el administrador de credenciales y escriba **Administrador de credenciales** en el cuadro de búsqueda de la barra de tareas y, a continuación, seleccione **Panel de control del administrador de credenciales**.</span><span class="sxs-lookup"><span data-stu-id="fe801-105">Open Credential Manager, and type **credential manager** in the search box on the taskbar, then select **Credential Manager Control panel**.</span></span>
1. <span data-ttu-id="fe801-106">Seleccione **credenciales de Windows**.</span><span class="sxs-lookup"><span data-stu-id="fe801-106">Select **Windows Credentials**.</span></span>
1. <span data-ttu-id="fe801-107">Busque cualquier entrada que empiece con la palabra **OneDrive**.</span><span class="sxs-lookup"><span data-stu-id="fe801-107">Find any entry that starts with the word **OneDrive**.</span></span>
1. <span data-ttu-id="fe801-108">Seleccione la entrada y, a continuación, presione **quitar**.</span><span class="sxs-lookup"><span data-stu-id="fe801-108">Select the entry, then press **Remove**.</span></span>
1. <span data-ttu-id="fe801-109">Cierre el administrador de credenciales, a continuación, haga clic con el botón secundario en la nube azul de la Systray y seleccione **cerrar OneDrive**.</span><span class="sxs-lookup"><span data-stu-id="fe801-109">Close Credential Manager, then right click on the blue cloud in your systray, and select **Close OneDrive**.</span></span>
1. <span data-ttu-id="fe801-110">Escriba **onedrive** en el cuadro de búsqueda de la barra de tareas y seleccione **aplicación de OneDrive** para iniciar onedrive.</span><span class="sxs-lookup"><span data-stu-id="fe801-110">Type **OneDrive** into the search box on the taskbar and select **OneDrive App** to launch OneDrive.</span></span>
1. <span data-ttu-id="fe801-111">Inicie sesión en OneDrive y, a continuación, intente guardar el archivo en OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fe801-111">Sign into OneDrive, then try to save the file to OneDrive.</span></span>
