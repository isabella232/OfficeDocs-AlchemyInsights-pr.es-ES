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
# <a name="issue-joining-vms"></a><span data-ttu-id="8a967-102">Problema al unir máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="8a967-102">Issue joining VMs</span></span>

<span data-ttu-id="8a967-103">Para resolver los problemas que se producen al intentar unir una máquina virtual, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="8a967-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="8a967-104">Pruebe a iniciar sesión con el formato **UPN** (por ejemplo, «usuariojose@contoso.com») en lugar de **SAMAccountName** («CONTOSO\usuariojose»).</span><span class="sxs-lookup"><span data-stu-id="8a967-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="8a967-105">Asegúrese de que ha habilitado la sincronización de contraseñas conforme a los pasos indicados en la guía *Introducción*.</span><span class="sxs-lookup"><span data-stu-id="8a967-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="8a967-106">Asegúrese de que la cuenta de usuario afectada no es una cuenta externa al espacio empresarial de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a967-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="8a967-107">Los usuarios externos no pueden iniciar sesión en el dominio administrado porque Azure AD Domain Services no tiene las credenciales de esas cuentas de usuario.</span><span class="sxs-lookup"><span data-stu-id="8a967-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="8a967-108">Si la cuenta de usuario afectada está basada solo en la nube, asegúrese de que los usuarios han cambiado la contraseña después de habilitar Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="8a967-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="8a967-109">Con este paso, se generan los hashes de credencial necesarios para Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="8a967-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="8a967-110">Si la cuenta de usuario afectada se sincroniza desde un directorio local, compruebe que la versión recomendada de Azure AD Connect se haya configurado para realizar una sincronización completa.</span><span class="sxs-lookup"><span data-stu-id="8a967-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="8a967-111">Si los problemas persisten después de confirmar el paso 4, ejecute los siguientes comandos desde su máquina de sincronización:</span><span class="sxs-lookup"><span data-stu-id="8a967-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="8a967-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="8a967-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>