---
title: Directiva de conexión de corrección
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314861"
---
# <a name="fix-connection-policy"></a>Directiva de conexión de corrección

El correo electrónico se marcó como seguro y se entregó a la Bandeja de entrada del usuario porque la dirección IP de origen se marcó como segura en la directiva de filtro de conexión predeterminada. Para revisar la directiva, siga estos pasos:

1. En el portal Microsoft 365 Defender en , vaya a Correo electrónico & directivas de colaboración & reglas directivas contra correo no deseado en <https://security.microsoft.com/>  \>  \>  \>  la **sección** Directivas.

   Para ir directamente a la página **Directivas contra correo no deseado**, use <https://security.microsoft.com/antispam>.

2. En la **página Directivas contra correo** no deseado, seleccione la directiva denominada Directiva de filtro de conexión **(predeterminada)** haciendo clic en el nombre de la directiva.

3. En el control desplegable de detalles que aparece, haga clic **en Editar directiva de filtro de conexión** en la sección Filtrado **de** conexiones.

4. Revise las entradas de la sección Permitir siempre mensajes de las siguientes **direcciones IP** o intervalo de direcciones y vea si activar **la lista** segura está seleccionada.

   **Nota:** Microsoft se suscribe a orígenes de terceros de remitentes de confianza. Si la lista segura está habilitada, estos remitentes de confianza no se marcan erróneamente como correo no deseado. Se recomienda seleccionar esta opción, ya que reducirá el número de falsos positivos (correo bueno que se clasifica como correo no deseado) que recibe.

Para obtener más información, consulte [Configurar filtrado de la conexión](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
