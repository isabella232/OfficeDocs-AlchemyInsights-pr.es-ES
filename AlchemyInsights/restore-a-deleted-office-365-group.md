---
title: Restaurar un grupo de Microsoft 365 eliminado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645148"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurar un grupo de Microsoft 365 eliminado

Puede restaurar un grupo eliminado de Microsoft 365 o Microsoft Teams en un plazo de 30 días desde la eliminación.

1. Vaya al [Centro de administración de Microsoft 365](https://aka.ms/RestoreDeletedGroup) para iniciar sesión en una lista de los grupos y equipos eliminados.

    **Nota:** Inicie sesión con la cuenta asignada al administrador de inquilinos o al rol de administrador de grupos.

1. Seleccione el grupo de Microsoft 365 eliminado/Teams que desea restaurar y haga clic en **Restaurar grupo**.

    Si el grupo no se puede restaurar debido a una dirección SMTP en conflicto, use el siguiente comando para buscar el objeto que está provocando conflictos y quitar la dirección SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Nota:** En algunos casos, el grupo y todos sus datos pueden tardar hasta 24 horas en restaurarse.

    Para obtener más información o aprender a restaurar grupos con PowerShell, vea [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).