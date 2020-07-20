---
title: Varios usuarios no ven los complementos en Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154606"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Varios usuarios no ven los complementos en Outlook

Si prueba los complementos de Outlook y no aparecen ninguno, como un primer paso de solución de problemas, use el cmdlet de PowerShell **Get-OrganizationConfig** para consultar el parámetro _AppsForOfficeEnabled_. Si la consulta devuelve un valor de **False**, establezca este parámetro en **True** con el cmdlet **Set-OrganizationConfig**, para que los complementos se muestren de la forma esperada.

No se recomienda establecer el parámetro _AppsForOfficeEnabled_ en **False**. Un valor **False** reemplaza todas las opciones de configuración de rol administrativo y de usuario anteriores y evita que todos los usuarios de la organización puedan activar aplicaciones nuevas.

Para obtener más información, consulte [Especifique los administradores y los usuarios que pueden instalar y administrar complementos para Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).