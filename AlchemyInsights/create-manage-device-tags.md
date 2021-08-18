---
title: Crear y administrar etiquetas de dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: c06ed00d7cf4bcb23fdcee12f446953918075728
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325666"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Crear y administrar etiquetas de dispositivos

Agregue etiquetas en los dispositivos para crear una afiliación de grupos lógica. Las etiquetas de dispositivo son compatibles con la asignación adecuada de la red, lo que permite adjuntar diferentes etiquetas para capturar contexto y habilitar la creación de listas dinámicas como parte de un incidente. Las etiquetas se pueden usar como filtro en la vista de lista de dispositivos o para agrupar dispositivos. Para obtener más información sobre la agrupación de dispositivos, consulte [Crear y administrar etiquetas de dispositivo](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags).

Puede agregar etiquetas en dispositivos de varias maneras:

- Usando el portal

- Estableciendo un valor de clave de registro
 
**Nota:** Podría haber una latencia entre el momento en que se agrega una etiqueta a un dispositivo y su disponibilidad en la lista de dispositivos y la página de dispositivos.

Para agregar etiquetas de dispositivo con la API, consulte [API para agregar o quitar etiquetas de dispositivo](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).

## <a name="add-and-manage-device-tags-using-the-portal"></a>Agregar y administrar etiquetas de dispositivo con el portal

1. Seleccione el dispositivo en el que quiere administrar las etiquetas. Puede seleccionar o buscar un dispositivo desde cualquiera de las siguientes vistas:

    - **Panel de operaciones de seguridad** Seleccione el nombre del dispositivo en la sección Dispositivos principales con alertas activas.
    - **Cola de alertas**: seleccione el nombre del dispositivo junto al icono de dispositivo en la cola de alertas.
    - **Lista de dispositivos**: seleccione el nombre del dispositivo de la lista de dispositivos.
    - **Cuadro de búsqueda**: seleccione Dispositivo en el menú desplegable y escriba el nombre del dispositivo.

    También puede acceder a la página de la alerta a través del archivo y las vistas IP.

1. Seleccione **Administrar etiquetas** en la fila Acciones de respuesta.

1. Escriba para buscar o crear etiquetas.

Las etiquetas se agregan a la vista de dispositivo y se reflejan en la vista de lista de dispositivos. Después podrá usar el filtro etiquetas para ver la lista de dispositivos relevante.

Para obtener más información, consulte [Crear y administrar etiquetas de dispositivo](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags).