---
title: Creación y uso compartido de calendarios de carpetas públicas en Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: 7ea393011d270fb342d09107f097fcfe685c67833d5a7106bf46b3c7fab0e352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080547"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a>Creación y uso compartido de calendarios de carpetas públicas en Exchange Online

Solo se puede crear un calendario en una carpeta pública desde el cliente de escritorio de Outlook. Siga estos pasos para configurar calendarios de carpetas públicas:

1. Compruebe que las carpetas públicas están implementadas en Exchange Online. Para obtener más información, consulte [Crear un buzón de carpetas públicas](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox). 

2. Compruebe que tiene asignados los permisos de acceso necesarios para crear la carpeta pública. Para obtener más información, consulte [Permisos de carpetas públicas de Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server). 
  
3. Inicie sesión en el cliente de escritorio de Outlook y compruebe que puede acceder a la implementación de la carpeta pública.

    Si tiene problemas para acceder a carpetas públicas con el cliente de escritorio de Outlook, consulte [Los usuarios de Exchange Online no se pueden conectar a carpetas públicas mediante Outlook o OWA](https://aka.ms/pfcte).

4. Cree un nuevo tipo de calendario para la carpeta pública.

La carpeta pública se comparte con el resto de usuarios de forma predeterminada. El propietario de la carpeta pública puede modificar los permisos desde el cliente de escritorio de Outlook. Para obtener más información, consulte [Permisos de carpetas públicas de Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).

**Nota:** Los calendarios de carpetas públicas están diseñados para usarse dentro de las organizaciones, por lo que no se pueden publicar en Internet. Use un buzón compartido si lo que quiere es publicar un calendario en Internet.