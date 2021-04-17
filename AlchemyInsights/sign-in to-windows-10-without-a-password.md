---
title: Iniciar sesión en Windows 10 sin usar una contraseña
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830563"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="dec23-102">Iniciar sesión en Windows 10 sin usar una contraseña</span><span class="sxs-lookup"><span data-stu-id="dec23-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="dec23-103">Para evitar tener que escribir una contraseña en el inicio de Windows, te recomendamos que uses una de las opciones de inicio de sesión seguro de Windows Hello, como un PIN, reconocimiento facial o huella digital, si está disponible.</span><span class="sxs-lookup"><span data-stu-id="dec23-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="dec23-104">Si realmente quieres deshabilitar el inicio de sesión seguro, consulta las instrucciones "Iniciar sesión automáticamente en Windows 10" a continuación.</span><span class="sxs-lookup"><span data-stu-id="dec23-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="dec23-105">**Alternativas seguras de Windows Hello a la contraseña de la cuenta**</span><span class="sxs-lookup"><span data-stu-id="dec23-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="dec23-106">Ve a **Configuración > cuentas > opciones de inicio** de sesión (o haz clic [aquí).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="dec23-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="dec23-107">Aparecerán las opciones de inicio de sesión disponibles.</span><span class="sxs-lookup"><span data-stu-id="dec23-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="dec23-108">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="dec23-108">For example:</span></span>

![Opciones de inicio de sesión.](media/sign-in-options.png)

<span data-ttu-id="dec23-110">Haga clic o pulse en una de las opciones para configurarla.</span><span class="sxs-lookup"><span data-stu-id="dec23-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="dec23-111">La próxima vez que inicies o desbloquees Windows, podrás usar la nueva opción en lugar de una contraseña.</span><span class="sxs-lookup"><span data-stu-id="dec23-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="dec23-112">**Iniciar sesión automáticamente en Windows 10**</span><span class="sxs-lookup"><span data-stu-id="dec23-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="dec23-113">**Nota:** El inicio de sesión automático es conveniente, pero presenta un riesgo de seguridad, especialmente si el equipo es accesible por varias personas.</span><span class="sxs-lookup"><span data-stu-id="dec23-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="dec23-114">Haga clic o pulse en **el botón** Inicio de la barra de tareas.</span><span class="sxs-lookup"><span data-stu-id="dec23-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="dec23-115">Escriba **netplwiz** y presione la tecla Entrar para abrir la ventana Cuentas de usuario.</span><span class="sxs-lookup"><span data-stu-id="dec23-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="dec23-116">En **Cuentas de usuario,** haz clic en la cuenta en la que quieres iniciar sesión automáticamente cuando se inicie Windows.</span><span class="sxs-lookup"><span data-stu-id="dec23-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="dec23-117">Desactive la casilla "Los usuarios deben escribir un nombre de usuario y una contraseña para usar este equipo".</span><span class="sxs-lookup"><span data-stu-id="dec23-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Los usuarios deben escribir una opción de nombre de usuario y contraseña.](media/users-must-enter-username.png)

5. <span data-ttu-id="dec23-119">Haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="dec23-119">Click **OK**.</span></span> <span data-ttu-id="dec23-120">Se le pedirá que escriba y confirme la contraseña de la cuenta que seleccionó.</span><span class="sxs-lookup"><span data-stu-id="dec23-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="dec23-121">Haga clic en **Aceptar** para finalizar.</span><span class="sxs-lookup"><span data-stu-id="dec23-121">Click **OK** to finish.</span></span> <span data-ttu-id="dec23-122">La próxima vez que se inicie Windows 10, iniciará sesión automáticamente en la cuenta seleccionada.</span><span class="sxs-lookup"><span data-stu-id="dec23-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
