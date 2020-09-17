---
title: Habilitar la escritura diferida en Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709744"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="4647f-102">Habilitar la escritura diferida en Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="4647f-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="4647f-103">Para habilitar el restablecimiento de contraseña de autoservicio, habilite primero la opción de reescritura en Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4647f-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="4647f-104">Desde el servidor de Azure AD Connect, siga los pasos que se indican a continuación:</span><span class="sxs-lookup"><span data-stu-id="4647f-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="4647f-105">Inicie sesión en el servidor de Azure AD Connect e inicie el **Asistente para la configuración de Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="4647f-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="4647f-106">En la página de **Bienvenida**, haga clic en **Configurar**.</span><span class="sxs-lookup"><span data-stu-id="4647f-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="4647f-107">En la página **Tareas adicionales**, haga clic en **Personalizar las opciones de sincronización** y, a continuación, haga clic en **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="4647f-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="4647f-108">En la página **Conectarse a Azure AD**, escriba una credencial de administrador global para su inquilino de Azure y haga clic en siguiente.</span><span class="sxs-lookup"><span data-stu-id="4647f-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="4647f-109">En las páginas **Conectar directorios** y **Filtrado de dominios y unidades organizativas**, haga clic en **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="4647f-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="4647f-110">En la página **Características opcionales**, seleccione la casilla junto a **Contraseña con escritura diferida** y haga clic en **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="4647f-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="4647f-111">En la página **Preparado para configurar**, haga clic en **Configurar** y espere a que finalice el proceso.</span><span class="sxs-lookup"><span data-stu-id="4647f-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="4647f-112">Cuando vea finalizar la configuración, haga clic en **Salir**.</span><span class="sxs-lookup"><span data-stu-id="4647f-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="4647f-113">Con la escritura a contraseña diferida en Azure AD Connect, ahora configure Azure AD SSPR para la reescritura.</span><span class="sxs-lookup"><span data-stu-id="4647f-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="4647f-114">Para habilitar la escritura diferida en SSPR, siga los pasos que se indican a continuación:</span><span class="sxs-lookup"><span data-stu-id="4647f-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="4647f-115">Inicie sesión en Microsoft Azure Portal con una cuenta de administrador global.</span><span class="sxs-lookup"><span data-stu-id="4647f-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="4647f-116">Busque y seleccione **Azure Active Directory**, haga clic en **Restablecer contraseña** y, a continuación, elija **Integración local**.</span><span class="sxs-lookup"><span data-stu-id="4647f-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="4647f-117">Establecer la opción de **¿Reescribir contraseñas en el directorio local?** en **Sí**.</span><span class="sxs-lookup"><span data-stu-id="4647f-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="4647f-118">Establecer la opción de **¿Permitir que los usuarios puedan desbloquear cuentas sin restablecer su contraseña?** a **Sí**.</span><span class="sxs-lookup"><span data-stu-id="4647f-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="4647f-119">Cuando haya terminado, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="4647f-119">When ready, click **Save**.</span></span>

<span data-ttu-id="4647f-120">Para obtener más información, consulte [Habilitar la reescritura diferida de la contraseña de autoservicio de Azure Active Directory en un entorno local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="4647f-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
