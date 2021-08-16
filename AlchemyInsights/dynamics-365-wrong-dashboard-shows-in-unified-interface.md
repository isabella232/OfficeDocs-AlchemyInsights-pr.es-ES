---
title: 'Dynamics 365: se muestra un panel incorrecto en la interfaz unificada de Dynamics 365'
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101499"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Se muestra un panel incorrecto en la interfaz unificada de Dynamics 365

Hay varias razones por las que puede ver un panel diferente del que espera:

## <a name="the-user-has-set-a-user-default-dashboard"></a>El usuario ha establecido un panel predeterminado del usuario 

Normalmente, se puede identificar un panel predeterminado del usuario si el botón **Establecer** como predeterminado no se muestra en la barra de comandos del panel. El panel predeterminado del usuario invalidará todos los demás paneles predeterminados, incluso si el panel predeterminado del usuario no está en la aplicación actual.

Use la siguiente solución alternativa para deshacer el panel predeterminado.

1. Cree un nuevo panel personal.

2. Establezca ese nuevo panel como el valor predeterminado del usuario.

3. Elimine ese panel.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>El panel se establece en el mapa del sitio

Es posible que haya establecido un panel predeterminado de la organización seleccionando un panel y seleccionando "Establecer como predeterminado" en "Personalizar el sistema". Pero el panel definido en el diseñador de mapa del sitio tendrá prioridad sobre este panel, si el usuario tiene acceso a él.

Para que los usuarios vean el panel que ha establecido como el valor predeterminado de la organización, puede:

* Establecer ese panel en el mapa del sitio

* Quitar el acceso al panel definido por el mapa del sitio para esos usuarios
