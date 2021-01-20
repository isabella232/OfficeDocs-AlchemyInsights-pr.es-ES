---
title: Problema al unir máquinas virtuales
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884614"
---
# <a name="issue-joining-vms"></a>Problema al unir máquinas virtuales

Para resolver los problemas que se producen al intentar unir una máquina virtual, siga estos pasos:

1. Pruebe a iniciar sesión con el formato **UPN** (por ejemplo, «usuariojose@contoso.com») en lugar de **SAMAccountName** («CONTOSO\usuariojose»).
2. Asegúrese de que ha habilitado la sincronización de contraseñas conforme a los pasos indicados en la guía *Introducción*.
3. Asegúrese de que la cuenta de usuario afectada no es una cuenta externa al espacio empresarial de Azure AD. Los usuarios externos no pueden iniciar sesión en el dominio administrado porque Azure AD Domain Services no tiene las credenciales de esas cuentas de usuario.
4. Si la cuenta de usuario afectada está basada solo en la nube, asegúrese de que los usuarios han cambiado la contraseña después de habilitar Azure AD Domain Services. Con este paso, se generan los hashes de credencial necesarios para Azure AD Domain Services.
5. Si la cuenta de usuario afectada se sincroniza desde un directorio local, compruebe que la versión recomendada de Azure AD Connect se haya configurado para realizar una sincronización completa.
6. Si los problemas persisten después de confirmar el paso 4, ejecute los siguientes comandos desde su máquina de sincronización:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.