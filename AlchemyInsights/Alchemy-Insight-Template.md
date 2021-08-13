---
title: igual que el nombre de archivo es mejor
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918918"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Encabezado de alquimia requerido H1, H2 no funciona".
Procedimientos recomendados y directrices para la creación de Alchemy:

1. **No anide Alchemy Ideas carpetas:** esto romperá la estructura de direcciones URL. Estamos buscando solucionar esto.
1. Los archivos de **la carpeta AlchemyInsights** deben tener nombres de archivo en minúsculas con guiones para espacios ex. **_how-to-enable-litigation-hold_**.
    1. Incluya el id. de regla o el id. de cubo del [portal de partners de Alchemy](https://alchemyportal.azurewebsites.net) en el campo ms.custom. ex. ***ms.custom: 100021***
1. Use el resto de los metadatos en la parte superior de este archivo como plantilla.
1. En el portal de partners de [Alchemy,](https://alchemyportal.azurewebsites.net)vaya a la sección Título de **customer insight:** y úselo como punto de partida para el título H1 para la información. 
    > [!NOTE]
    > Alchemy Ideas debe tener un solo H1 en la parte superior o interrumpirán la producción. H2s don't render either so use **bold** or other conventions to signify separate sections.
1. A continuación, rellene el texto del cuerpo con el material de borrador en la Customer Insights de la página Regla de alquimia
    1. Las listas con viñetas están bien
    1. Listas numeradas también
    1. **Negrita** y *cursiva* son a-ok
    1. Los vínculos siempre deben ser **"vínculos a web"/externos** o vínculos profundos **a** elementos de la interfaz de usuario, no vínculos internos.
    1. Las imágenes no se admiten oficialmente en este momento, pero está en la hoja de ruta.

Y esto ya es demasiado largo. El procedimiento recomendado es de unos 400 ---------------------------------

Una vez que el contenido esté listo, eléctelo a la rama en directo. A continuación, vaya al [portal de partners de Alchemy](https://alchemyportal.azurewebsites.net) y escriba el nombre de archivo en el campo url. 