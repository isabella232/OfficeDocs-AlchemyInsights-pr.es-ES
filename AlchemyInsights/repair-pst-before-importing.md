---
title: Reparar el archivo. pst antes de importar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799113"
---
# <a name="repair-pst-file-before-importing"></a>Reparar el archivo. pst antes de importar

Antes de importar un archivo. pst en Outlook, compruebe que el archivo no está dañado reparando el archivo:

1. Cierre Outlook.

2. Busque y ejecute `Scanpst.exe` en la carpeta del programa de Office (C:\Program Files (x86) \Microsoft Office\root\Office \<Version\> o C:\Archivos de programa\Microsoft Office\root\Office \<Version\> ).

3. En la **herramienta de reparación de la bandeja de entrada de Microsoft Outlook**, haga clic en **examinar** para buscar el archivo. pst (por ejemplo, en C:\Users \\<nombredeusuario \> \AppData\Local\Microsoft\Outlook). Seleccione el archivo. PST y, a continuación, haga clic en **abrir**.

4. Haga clic en **iniciar** para iniciar el análisis.

5. Si se encuentran errores en el archivo, haga clic en **reparar**y, a continuación, haga clic en **Aceptar** cuando se complete la reparación.

6. Intente volver a importar el archivo. pst en Outlook.

Para obtener más información, vea [reparar archivos de datos de Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) y [solucionar problemas al importar un archivo. pst de Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
