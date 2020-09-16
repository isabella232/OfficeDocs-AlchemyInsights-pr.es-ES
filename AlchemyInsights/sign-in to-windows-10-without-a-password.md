---
title: Iniciar sesión en Windows 10 sin usar una contraseña
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719970"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="cb5c0-102">Iniciar sesión en Windows 10 sin usar una contraseña</span><span class="sxs-lookup"><span data-stu-id="cb5c0-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="cb5c0-103">Para evitar tener que escribir una contraseña durante el inicio de Windows, le recomendamos que use una de las opciones de inicio de sesión seguro de Windows Hello, como un PIN, un reconocimiento facial o una huella digital, si está disponible.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="cb5c0-104">Si realmente quiere deshabilitar el inicio de sesión seguro, consulte las instrucciones "iniciar sesión automáticamente en Windows 10" a continuación.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="cb5c0-105">**Proteger las alternativas de Windows Hello a la contraseña de la cuenta**</span><span class="sxs-lookup"><span data-stu-id="cb5c0-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="cb5c0-106">Vaya a **configuración > cuentas > opciones de inicio de sesión** (o haga clic [aquí](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="cb5c0-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="cb5c0-107">Se mostrarán las opciones de inicio de sesión disponibles.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="cb5c0-108">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="cb5c0-108">For example:</span></span>

![Opciones de inicio de sesión.](media/sign-in-options.png)

<span data-ttu-id="cb5c0-110">Haga clic o pulse en una de las opciones para configurarla.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="cb5c0-111">La siguiente vez que inicie o desbloquee Windows, podrá usar la nueva opción en lugar de una contraseña.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="cb5c0-112">**Inicio de sesión automático en Windows 10**</span><span class="sxs-lookup"><span data-stu-id="cb5c0-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="cb5c0-113">**Nota**: el inicio de sesión automático es conveniente, pero introduce un riesgo de seguridad, especialmente si el equipo es accesible para varias personas.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="cb5c0-114">Haga clic o pulse en el botón **Inicio** de la barra de tareas.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="cb5c0-115">Escriba **netplwiz** y presione la tecla entrar para abrir la ventana cuentas de usuario.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="cb5c0-116">En **cuentas de usuario**, haga clic en la cuenta en la que desea iniciar sesión automáticamente cuando se inicie Windows.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="cb5c0-117">Desactive la casilla "los usuarios deben escribir un nombre de usuario y una contraseña para usar el equipo".</span><span class="sxs-lookup"><span data-stu-id="cb5c0-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Los usuarios deben escribir una opción de nombre de usuario y contraseña.](media/users-must-enter-username.png)

5. <span data-ttu-id="cb5c0-119">Haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-119">Click **OK**.</span></span> <span data-ttu-id="cb5c0-120">Se le pedirá que escriba y confirme la contraseña de la cuenta que ha seleccionado.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="cb5c0-121">Haga clic en **Aceptar** para finalizar.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-121">Click **OK** to finish.</span></span> <span data-ttu-id="cb5c0-122">La próxima vez que se inicie Windows 10, se iniciará sesión automáticamente en la cuenta seleccionada.</span><span class="sxs-lookup"><span data-stu-id="cb5c0-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
