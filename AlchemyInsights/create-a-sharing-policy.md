---
title: Creación de una directiva de uso compartido para permitir que los usuarios compartan sus calendarios con personas fuera de su organización
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
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816289"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a>Creación de una directiva de uso compartido para permitir que los usuarios compartan sus calendarios con personas fuera de su organización

1. En el panel del Centro de administración de Microsoft 365, vaya a **Administración** > **Exchange**.
2. Vaya a **Organización** > **Uso compartido**.
3. En la vista de lista, en **Uso compartido individual**, haga clic en **Nuevo**.
4. En **Nueva directiva compartida**, escriba un nombre descriptivo para la directiva de uso compartido en el cuadro **Nombre de la directiva**.
5. Haga clic en **Agregar** para definir las reglas de uso compartido de la directiva.
6. En **regla de uso compartido**, seleccione una de las siguientes opciones para especificar los dominios con los que desea compartir:
    - **Compartir con todos los dominios**
    - **Compartir con un dominio específico**
8. Si selecciona **Compartir con un dominio específico**, escriba el dominio con el que desea compartir. Si necesita indicar más de un dominio para esta directiva de uso compartido, guarde la configuración del primer dominio y, después, cambie las reglas de uso compartido para agregar más dominios.
9. Para especificar la información que se va a poder compartir, active la casilla **Compartir la carpeta de calendario** y, a continuación, seleccione una de las siguientes opciones:
    - **Información de disponibilidad de calendario solo con hora**
    - **Información de disponibilidad de calendario con hora, asunto y ubicación**
    - **Toda la información de citas de calendarios, incluidas la hora, el asunto, la ubicación y el título**
11. Haga clic en **guardar** para configurar las reglas de la directiva de uso compartido.
12. Si quiere establecer esta directiva de uso compartido como nueva directiva predeterminada para todos los usuarios de la organización, active la casilla **Hacer que esta sea mi directiva de uso compartido predeterminada**.
13. Haga clic en **Guardar** para crear la directiva de uso compartido.  

**Para comprender completamente este tema, lea:**

- [Crear una directiva de uso compartido en Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [Aplicar una directiva de uso compartido a buzones de correo en Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [Modificar, deshabilitar o quitar una directiva de uso compartido en Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)