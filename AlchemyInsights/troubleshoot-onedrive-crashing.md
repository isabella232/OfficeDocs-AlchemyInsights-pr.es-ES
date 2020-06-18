---
title: Solución de problemas de bloqueo de OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/15/2020
ms.locfileid: "44735398"
---
# <a name="troubleshoot-onedrive-crashes"></a>Solución de problemas de bloqueo de OneDrive

Si OneDrive se bloquea de forma repetida, pruebe estos pasos de solución de problemas:

**Asegúrese de que las claves del registro no estén configuradas:**

1. Abra el Editor del Registro y vaya a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Si existe la clave DisableFileSyncNGSC y esta está establecida en 1, abra la clave y cambie el valor a 0.
3. Vaya a Inicio para iniciar OneDrive manualmente. ![Presione la tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), escriba OneDrive en el cuadro de búsqueda y luego haga clic en la aplicación de escritorio de OneDrive.

**Restablezca OneDrive:**

Notas:

- Al restablecer OneDrive, todas las conexiones de sincronización existentes se desconectarán (incluida la de OneDrive personal, si está configurada).
- Si restablece OneDrive en su equipo, no perderá sus archivos ni su información.

**Para restablecer OneDrive:**

1. Presione las teclas Windows y R para abrir el cuadro de diálogo Ejecutar.
2. Escriba %localappdata%\Microsoft\OneDrive\onedrive.exe/reset y presione Aceptar. Es posible que aparezca momentáneamente una ventana de comandos.
3. Vaya a Inicio para iniciar OneDrive manualmente. ![Presione la tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), escriba OneDrive en el cuadro de búsqueda y luego haga clic en la aplicación de escritorio de OneDrive.

Notas:

- Si antes del restablecimiento elige sincronizar solo algunas carpetas, deberá hacerlo de nuevo una vez que se haya completado la sincronización. Lea  [Elegir qué carpetas de OneDrive se sincronizarán con su equipo](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) para obtener más información.
- Tendrá que seguir estos pasos con su OneDrive personal y con OneDrive para la Empresa.