---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043223"
---
# <a name="how-to-import-nk2-files"></a>Cómo importar archivos .nk2 

Al iniciar Microsoft Outlook 2013, Outlook 2016, Outlook 2019 o Outlook para Microsoft 365 por primera vez, la caché de alias (almacenada en el archivo *profilename*.nk2) se importa en un mensaje oculto en el almacén de mensajes predeterminado.

Para importar archivos .nk2 a Outlook 2013, Outlook 2016, Outlook 2019 o Outlook para Microsoft 365, asegúrese de que el archivo .nk2 se encuentra en la carpeta siguiente: %appdata%\Microsoft\Outlook

**Nota:** El archivo .nk2 debe tener el mismo nombre que el nombre actual Outlook 2013 o Outlook 2016 perfil. De forma predeterminada, el nombre del perfil es "Outlook". Para comprobar el nombre del perfil, siga estos pasos: 
1. Haga clic en **Inicio** y en **Panel de control**.
2. Haga doble clic en **Mail**.
3. En el cuadro de diálogo Configuración de correo, seleccione **Mostrar perfiles**.
4. Seleccione **Inicio** > **Ejecutar**.
5. En el **cuadro** Abrir, *escribaoutlook.exe /importnk2* y, a continuación, seleccione **Aceptar**. 

Después de importar el archivo .nk2, el contenido del archivo se combina con la caché de alias existente almacenada en el buzón.

**Nota:** El nombre del archivo .nk2 se cambia por una extensión de nombre de archivo .old la próxima vez que inicie Outlook 2013, Outlook 2016, Outlook 2019 o Outlook para Microsoft 365. Si desea volver a importar el archivo .nk2, quite primero la extensión de nombre de archivo .old.

Para obtener más información, [vea Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).