---
title: Corregir directiva de inquilino (invalidación de acción)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326814"
---
# <a name="fix-tenant-policy-action-override"></a>Corregir directiva de inquilino (invalidación de acción)

Una de las directivas contra correo no deseado afectó a este mensaje. Para revisar las directivas, siga estos pasos:

1. En el portal Microsoft 365 Defender en , vaya a Correo electrónico & directivas de colaboración & reglas directivas contra correo no deseado en <https://security.microsoft.com/>  \>  \>  \>  la **sección** Directivas.

   Para ir directamente a la página **Directivas contra correo no deseado**, use <https://security.microsoft.com/antispam>.

2. En la página **Directivas** contra correo no deseado, seleccione la directiva  haciendo clic en  el nombre de la directiva **(** Tipo es Directiva contra correo no deseado personalizada o Nombre es Directiva de entrada contra correo no deseado **(valor predeterminado).**
3. En el control desplegable de detalles que aparece, seleccione **Editar acciones** en la **sección** Acciones.
4. En la **sección Acciones del** mensaje, revise los veredictos de correo no deseado, correo no deseado de elevada confianza, suplantación de identidad   **(phishing)** y **suplantación** de identidad de confianza alta para ver si se selecciona alguno de los siguientes valores:
   - **Agregar encabezado X**
   - **Anteponer texto a la línea de asunto**
   - **Redirigir el mensaje a la dirección de correo electrónico**
   - **Eliminar mensaje**
   - **Ninguna acción**

   Es posible que la configuración estándar **aplicada** a todos los clientes Exchange Online Protection afectaron al mensaje.

Para más información, consulte [Configurar directivas contra correo electrónico no deseado en EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
