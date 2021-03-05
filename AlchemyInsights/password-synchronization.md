---
title: Sincronización de contraseña
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449168"
---
# <a name="password-synchronization"></a>Sincronización de contraseña

**La sincronización de hash de contraseña no funciona en absoluto**

Algunos problemas comunes que los clientes encuentran cuando la sincronización de hash de contraseña no funciona son:

- A la cuenta de Active Directory usada por Azure AD  Connect para  comunicarse con Active Directory local no se le concede Replicar cambios de directorio y Replicar cambios de directorio Todos los permisos, que son necesarios para la sincronización de contraseñas: debe corregir esto concediendo estos permisos a la cuenta de Active Directory.
- La sincronización de hash de contraseña está deshabilitada  después de que un administrador haya cambiado el método User Sign-In de Sincronización de contraseñas a otra opción, como Federación con **AD FS** en el Asistente para Azure AD Connect: puede solucionar esto si vuelve a habilitar la característica de sincronización de **hash** de contraseña en el Asistente para Azure AD Connect.
- Problema de conectividad con Active Directory local. Por ejemplo, Azure AD Connect no puede tener [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) acceso a algunos controladores de dominio o los puertos requeridos están bloqueados por firewall: debe solucionarlo asegurándose de que la conectividad entre el servidor de Azure AD Connect y el Active Directory local funcione correctamente.
- Servidor de Azure AD Connect que se encuentra actualmente en modo provisional, lo que provocará que el servidor no pueda usar los hashes de contraseña: para solucionar el problema, siga los pasos descritos en la sección Solucionar problemas de sincronización de contraseñas con sincronización de [Azure AD Connect: no](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)se sincronizan contraseñas.

**La sincronización de hash de contraseña no funciona para algunos de mis usuarios**

1. Si notaste que el hash de contraseña no  se está sincronizando para un usuario, usa la tarea de solución de problemas en Azure AD Connect para investigar y resolver el problema. Realice las siguientes tareas:

    a. [Ejecutar la tarea de solución de problemas en el asistente](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Usar el cmdlet de solución de problemas para investigar el problema de sincronización de hash de contraseña para un uso específico](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. El objeto de usuario de Active Directory local está habilitado para que el usuario **cambie la contraseña en la siguiente** opción de inicio de sesión. Cuando esta opción está habilitada, al usuario se le asigna una contraseña temporal y se le pedirá que cambie la contraseña en el siguiente inicio de sesión. Azure AD Connect no sincroniza contraseñas temporales con Azure AD.

Para resolver el problema anterior, realice una de las siguientes tareas:

- Pida al usuario que inicie sesión en la aplicación local (por ejemplo, Windows Desktop) y cambie la contraseña. La nueva contraseña se sincronizará con Azure AD.
- Haga que un administrador actualice la contraseña del usuario sin habilitar la opción El usuario debe cambiar la contraseña en el siguiente inicio de sesión **y** compartir la nueva contraseña con el usuario.

3. El objeto user de Active Directory local no **está configurado correctamente para** la sincronización de objetos o la sincronización de contraseñas. Para solucionar este problema, siga los pasos descritos en Troubleshoot [password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







