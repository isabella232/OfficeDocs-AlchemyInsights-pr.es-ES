---
title: Establecer Microsoft Edge como el explorador web predeterminado en un dispositivo unido a un dominio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426893"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Establecer Microsoft Edge como el explorador web predeterminado en un dispositivo unido a un dominio

Establecer Microsoft Edge como explorador web predeterminado: 

1. [Cree un archivo de configuración de asociaciones predeterminado](https://go.microsoft.com/fwlink/?linkid=2132437) y guárdelo localmente o en un recurso compartido de red.

1. Abra el editor de Directivas de grupo y a continuación, vaya a **Configuración del equipo** > **Plantillas administrativas** > **Componentes de Windows** > **Explorador de archivos**.

1. Seleccione **Establecer un archivo de configuración de asociaciones predeterminado**.

1. Seleccione **Configuración de directivas** y después seleccione **Habilitado**.

1. En **Opciones**, escriba la ubicación del archivo de configuración de asociaciones predeterminado y, a continuación, seleccione **Aceptar**.
