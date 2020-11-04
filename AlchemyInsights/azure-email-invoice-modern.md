---
title: Facturación moderna de correo electrónico de Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840630"
---
# <a name="email-invoicing-in-azure"></a>Facturación de correo electrónico en Azure

Debes tener un rol de propietario o colaborador en el perfil de facturación o en su cuenta de facturación para actualizar su preferencia de facturación por correo electrónico. Una vez que haya optado por recibir, todos los usuarios con funciones de propietario, colaborador, lector y gestor de facturas en un perfil de facturación recibirán su factura por correo electrónico.

1. Inicie sesión en el [portal de Azure](https://portal.azure.com/).
2. Buscar la **administración de costos + facturación**.
3. Seleccione **Facturas** en la parte izquierda y, a continuación, seleccione **Factura de correo electrónico** desde la parte superior de la página.
4. Si tiene varios perfiles de facturación, seleccione un perfil de facturación y, a continuación, seleccione **optar por recibir**.

5. Seleccione **Actualizar**.
6. Si tiene varios perfiles de facturación, seleccione un perfil de facturación y, a continuación, seleccione **optar por recibir**.

Para conceder acceso a otros usuarios para ver, descargar y pagar facturas, debe asignarles el rol de administrador de facturas para un perfil de facturación MCA o MPA. Si ha optado por recibir su factura en el correo electrónico, los usuarios también recibirán las facturas por correo electrónico.

1. Inicie sesión en el [portal de Azure](https://portal.azure.com/).
2. Buscar la **administración de costos + facturación**.
3. Seleccione **perfiles de facturación** en la parte izquierda. En la lista perfiles de facturación, seleccione un perfil de facturación al que quiera asignar un rol de administrador de facturas.
4. Seleccione **Access Control (IAM)** desde el lado izquierdo y, a continuación, seleccione **Agregar** desde la parte superior de la página.

En la lista desplegable Rol, seleccione **administrador de facturas**. Escriba la dirección de correo electrónico del usuario para dar acceso. Seleccione **Guardar** para asignar el rol.
