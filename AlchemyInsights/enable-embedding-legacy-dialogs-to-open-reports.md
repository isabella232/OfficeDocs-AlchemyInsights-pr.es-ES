---
title: Habilitar la incrustación de cuadros de diálogo heredados para abrir informes
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003406"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Habilitar la incrustación de cuadros de diálogo heredados para abrir informes

**Síntoma**

Los usuarios no pueden abrir los informes. "Algo ha fallado. Compruebe los detalles técnicos para obtener más información".

**Causa**

No se pueden cargar los informes en UCI con el error: "El descriptor del formulario es nulo o no está definido". Los informes en UCI aún requieren cuadros de diálogo heredados, por lo que el sistema del cliente debe tener *allowlegacydialogsembedding* habilitado.

**Solución**

1. Vaya a **Configuración > Administración > Configuración del sistema > pestaña General**.

2. Establezca la opción "Habilitar la incrustación de determinados cuadros de diálogo heredados en el cliente unificado del explorador de interfaces" en **Sí**.
