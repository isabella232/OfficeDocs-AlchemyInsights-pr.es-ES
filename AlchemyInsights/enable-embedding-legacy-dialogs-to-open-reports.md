---
title: Habilitar la incrustación de cuadros de diálogo heredados para abrir informes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806452"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Habilitar la incrustación de cuadros de diálogo heredados para abrir informes

**Síntoma**

Los usuarios no pueden abrir los informes. "Algo ha fallado. Compruebe los detalles técnicos para obtener más información".

**Causa**

No se pueden cargar los informes en UCI con el error: "El descriptor del formulario es nulo o no está definido". Los informes en UCI aún requieren cuadros de diálogo heredados, por lo que el sistema del cliente debe tener *allowlegacydialogsembedding* habilitado.

**Solución**

1. Vaya a **Configuración > Administración > Configuración del sistema > pestaña General**.

2. Establezca la opción "Habilitar la incrustación de determinados cuadros de diálogo heredados en el cliente unificado del explorador de interfaces" en **Sí**.
