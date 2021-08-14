---
title: Restaurar un grupo Microsoft 365 eliminado
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959043"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurar un grupo Microsoft 365 eliminado

Puede restaurar un grupo de Microsoft 365 eliminado o Microsoft Teams dentro de los 30 días siguientes a la eliminación.

1. Vaya a la [Centro de administración de Microsoft 365](https://aka.ms/RestoreDeletedGroup) para iniciar sesión en una lista de los grupos y equipos eliminados.

    **Nota:** Inicie sesión con la cuenta asignada al administrador de inquilinos o al rol de administrador de grupos.

1. Seleccione el grupo Microsoft 365 o Teams que desea restaurar y haga clic en **Restaurar grupo**.

    Si el grupo no se puede restaurar debido a una dirección SMTP en conflicto, use el siguiente comando para buscar el objeto que está provocando conflictos y quitar la dirección SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Nota:** En algunos casos, el grupo y todos sus datos pueden tardar hasta 24 horas en restaurarse.

    Para obtener más información o para obtener información sobre cómo restaurar grupos con PowerShell, vea [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).