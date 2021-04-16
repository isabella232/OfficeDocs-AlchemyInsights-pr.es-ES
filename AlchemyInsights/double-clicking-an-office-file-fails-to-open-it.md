---
title: Al hacer doble clic en un archivo de Office no se puede abrir
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
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814822"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Al hacer doble clic en un archivo de Office no se puede abrir

Después de hacer doble clic en un archivo de Office, es posible que vea el programa abierto, pero el archivo en sí no se abre. O puede obtener el error: "Hubo un problema al enviar el comando al programa". Hay muchas causas para esto, pero las dos soluciones más comunes son:

- Desde Excel, asegúrese de que la opción DDE está desactivada. La opción se puede encontrar mediante la creación de un nuevo libro y, a continuación, eligiendo **Archivo > opciones > advanced**. En la **sección General,** desactive omitir otras aplicaciones que **usan Dynamic Data Exchange (DDE).**

- Ejecute una reparación en línea para restaurar la configuración predeterminada. Haz clic en el botón Inicio de Windows y busca "Panel de control". Abra el **Panel de control** y vaya a Programas > y **características**. A continuación, **haga clic Microsoft Office [Versión]** y elija **Cambiar > Reparación en línea**.

Si ninguna de estas soluciones funciona, se puede encontrar una lista más completa de soluciones en el artículo de soporte técnico, al hacer doble clic en un archivo de [Office no](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)se puede abrir .
