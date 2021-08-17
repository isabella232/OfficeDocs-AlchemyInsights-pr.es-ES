---
title: 'Error: no podemos cargar ni descargar los cambios porque las credenciales almacenadas en caché han expirado'
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
ms.openlocfilehash: 623c2f1175ed2ab9638e742521395fe62ba9cad9d21b517f17426fb5c96a2d73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059459"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a>Error: no podemos cargar ni descargar los cambios porque las credenciales almacenadas en caché han expirado

Al guardar archivos en la aplicación OneDrive, si recibe un error que contiene la frase "las credenciales almacenadas en caché han **expirado",** siga estos pasos:

1. Cierre todas las aplicaciones de Office.
1. Abra Credential Manager y escriba **administrador** de credenciales en el cuadro de búsqueda de la barra de tareas y, a continuación, seleccione **Panel de control de Credential Manager**.
1. Seleccione **Windows credenciales**.
1. Busque cualquier entrada que comience con la palabra **OneDrive**.
1. Seleccione la entrada y, a continuación, **presione Quitar**.
1. Cierre Credential Manager, haga clic con el botón secundario en la nube azul de su systray y seleccione **Cerrar OneDrive**.
1. Escribe **OneDrive** en el cuadro de búsqueda de la barra de tareas y selecciona **OneDrive app** para iniciar OneDrive.
1. Inicie sesión OneDrive y, a continuación, intente guardar el archivo en OneDrive.
