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
ms.openlocfilehash: ba46da6d67bbfd602d8e5f3fa03d0e607ba3243ad4b9b592b09b606c73fa8f44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921780"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Establecer Microsoft Edge como el explorador web predeterminado en un dispositivo unido a un dominio

Establecer Microsoft Edge como explorador web predeterminado: 

1. [Cree un archivo de configuración de asociaciones predeterminado](https://go.microsoft.com/fwlink/?linkid=2132437) y guárdelo localmente o en un recurso compartido de red.

1. Abra el editor de Directivas de grupo y a continuación, vaya a **Configuración del equipo** > **Plantillas administrativas** > **Componentes de Windows** > **Explorador de archivos**.

1. Seleccione **Establecer un archivo de configuración de asociaciones predeterminado**.

1. Seleccione **Configuración de directivas** y después seleccione **Habilitado**.

1. En **Opciones**, escriba la ubicación del archivo de configuración de asociaciones predeterminado y, a continuación, seleccione **Aceptar**.
