---
title: SharePoint listas grandes
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941637"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Trabajar con listas y bibliotecas grandes en SharePoint

SharePoint listas y bibliotecas pueden contener hasta 30 millones de elementos, pero cuando tienen más de 5.000 elementos, es posible que vea un error de umbral de vista de lista al intentar trabajar con ellos. Se ha establecido este umbral para mantener el rendimiento del servicio. No se puede cambiar. Para evitar alcanzar este umbral:

**Usar moderno**

Las vistas que muestran muchos elementos funcionan mejor en la experiencia moderna. [Usa la experiencia moderna para](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) evitar errores que podrías ver en la experiencia clásica.

**Agregar índices**

Al filtrar u ordenar por una columna que no tiene un índice, es posible que vea un mensaje de error. [Agregue un índice](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manualmente desde **Lista Configuración** en el menú configuración y, a continuación, **Columnas indizadas**.

**Editar la vista de lista**

Si se produce un error al trabajar con una lista grande, [edite la vista de lista](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Los cuatro cambios siguientes quitarán los errores de umbral de vista de lista. Realice los cuatro cambios para quitar todos los errores. Si sigue recibiendo errores, compruebe [Administrar listas y bibliotecas grandes.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Seleccione **Ninguno** de **la primera ordenación por columna** y, a **continuación, ordene por la columna**.
2. Seleccione **Ninguno** de los dos **grupos First por la columna** y Then group by the **column**.
3. Seleccione **Ninguno** para todas las columnas en la **sección Totales.**
4. Anule la selección de todas las columnas menos una para mostrar en la **sección** Columnas.

