---
title: Varios usuarios no ven los complementos en Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729888"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Varios usuarios no ven los complementos en Outlook

Si prueba los complementos de Outlook y no aparecen ninguno, como un primer paso de solución de problemas, use el cmdlet de PowerShell **Get-OrganizationConfig** para consultar el parámetro _AppsForOfficeEnabled_. Si la consulta devuelve un valor de **False**, establezca este parámetro en **True** con el cmdlet **Set-OrganizationConfig**, para que los complementos se muestren de la forma esperada.

No se recomienda establecer el parámetro _AppsForOfficeEnabled_ en **False**. Un valor **False** reemplaza todas las opciones de configuración de rol administrativo y de usuario anteriores y evita que todos los usuarios de la organización puedan activar aplicaciones nuevas.

Para obtener más información, consulte [Especifique los administradores y los usuarios que pueden instalar y administrar complementos para Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).