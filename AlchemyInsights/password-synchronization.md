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
# <a name="password-synchronization"></a><span data-ttu-id="61a77-102">Sincronización de contraseña</span><span class="sxs-lookup"><span data-stu-id="61a77-102">Password synchronization</span></span>

<span data-ttu-id="61a77-103">**La sincronización de hash de contraseña no funciona en absoluto**</span><span class="sxs-lookup"><span data-stu-id="61a77-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="61a77-104">Algunos problemas comunes que los clientes encuentran cuando la sincronización de hash de contraseña no funciona son:</span><span class="sxs-lookup"><span data-stu-id="61a77-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="61a77-105">A la cuenta de Active Directory usada por Azure AD  Connect para  comunicarse con Active Directory local no se le concede Replicar cambios de directorio y Replicar cambios de directorio Todos los permisos, que son necesarios para la sincronización de contraseñas: debe corregir esto concediendo estos permisos a la cuenta de Active Directory.</span><span class="sxs-lookup"><span data-stu-id="61a77-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="61a77-106">La sincronización de hash de contraseña está deshabilitada  después de que un administrador haya cambiado el método User Sign-In de Sincronización de contraseñas a otra opción, como Federación con **AD FS** en el Asistente para Azure AD Connect: puede solucionar esto si vuelve a habilitar la característica de sincronización de **hash** de contraseña en el Asistente para Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="61a77-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="61a77-107">Problema de conectividad con Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="61a77-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="61a77-108">Por ejemplo, Azure AD Connect no puede tener [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) acceso a algunos controladores de dominio o los puertos requeridos están bloqueados por firewall: debe solucionarlo asegurándose de que la conectividad entre el servidor de Azure AD Connect y el Active Directory local funcione correctamente.</span><span class="sxs-lookup"><span data-stu-id="61a77-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="61a77-109">Servidor de Azure AD Connect que se encuentra actualmente en modo provisional, lo que provocará que el servidor no pueda usar los hashes de contraseña: para solucionar el problema, siga los pasos descritos en la sección Solucionar problemas de sincronización de contraseñas con sincronización de [Azure AD Connect: no](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)se sincronizan contraseñas.</span><span class="sxs-lookup"><span data-stu-id="61a77-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="61a77-110">**La sincronización de hash de contraseña no funciona para algunos de mis usuarios**</span><span class="sxs-lookup"><span data-stu-id="61a77-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="61a77-111">Si notaste que el hash de contraseña no  se está sincronizando para un usuario, usa la tarea de solución de problemas en Azure AD Connect para investigar y resolver el problema.</span><span class="sxs-lookup"><span data-stu-id="61a77-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="61a77-112">Realice las siguientes tareas:</span><span class="sxs-lookup"><span data-stu-id="61a77-112">Perform the following tasks:</span></span>

    <span data-ttu-id="61a77-113">a.</span><span class="sxs-lookup"><span data-stu-id="61a77-113">a.</span></span> [<span data-ttu-id="61a77-114">Ejecutar la tarea de solución de problemas en el asistente</span><span class="sxs-lookup"><span data-stu-id="61a77-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="61a77-115">b.</span><span class="sxs-lookup"><span data-stu-id="61a77-115">b.</span></span> [<span data-ttu-id="61a77-116">Usar el cmdlet de solución de problemas para investigar el problema de sincronización de hash de contraseña para un uso específico</span><span class="sxs-lookup"><span data-stu-id="61a77-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="61a77-117">El objeto de usuario de Active Directory local está habilitado para que el usuario **cambie la contraseña en la siguiente** opción de inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="61a77-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="61a77-118">Cuando esta opción está habilitada, al usuario se le asigna una contraseña temporal y se le pedirá que cambie la contraseña en el siguiente inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="61a77-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="61a77-119">Azure AD Connect no sincroniza contraseñas temporales con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="61a77-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="61a77-120">Para resolver el problema anterior, realice una de las siguientes tareas:</span><span class="sxs-lookup"><span data-stu-id="61a77-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="61a77-121">Pida al usuario que inicie sesión en la aplicación local (por ejemplo, Windows Desktop) y cambie la contraseña.</span><span class="sxs-lookup"><span data-stu-id="61a77-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="61a77-122">La nueva contraseña se sincronizará con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="61a77-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="61a77-123">Haga que un administrador actualice la contraseña del usuario sin habilitar la opción El usuario debe cambiar la contraseña en el siguiente inicio de sesión **y** compartir la nueva contraseña con el usuario.</span><span class="sxs-lookup"><span data-stu-id="61a77-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="61a77-124">El objeto user de Active Directory local no **está configurado correctamente para** la sincronización de objetos o la sincronización de contraseñas.</span><span class="sxs-lookup"><span data-stu-id="61a77-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="61a77-125">Para solucionar este problema, siga los pasos descritos en Troubleshoot [password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="61a77-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







