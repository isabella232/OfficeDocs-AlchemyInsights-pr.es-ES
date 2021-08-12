---
title: Al hacer doble clic en un Office no se puede abrir.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965118"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Al hacer doble clic en un Office no se puede abrir.

Después de hacer doble clic en Office archivo, es posible que vea el programa abierto, pero el archivo en sí no se abre. O puede obtener el error: "Hubo un problema al enviar el comando al programa". Hay muchas causas para esto, pero las dos soluciones más comunes son:

- Desde dentro Excel, asegúrese de que la opción DDE está desactivada. La opción se puede encontrar mediante la creación de un nuevo libro y, a continuación, eligiendo **Archivo > opciones > advanced**. En la **sección General,** desactive omitir otras aplicaciones que usan **datos dinámicos Exchange (DDE).**

- Ejecute una reparación en línea para restaurar la configuración predeterminada. Haga clic en Windows botón Inicio y busque "Panel de control". Abra el **Panel de control** y vaya a Programas > y **características**. A continuación, **haga clic Microsoft Office [Versión]** y elija **Cambiar > Reparación en línea**.

Si ninguna de estas soluciones funciona, se puede encontrar una lista más completa de soluciones en el artículo de soporte técnico, al hacer doble clic en un archivo Office no se puede [abrir](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
