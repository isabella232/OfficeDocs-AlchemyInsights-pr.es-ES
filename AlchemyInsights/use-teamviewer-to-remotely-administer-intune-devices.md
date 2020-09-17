---
title: Use TeamViewer para administrar dispositivos Intune de manera remota
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798465"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="89adf-102">Use TeamViewer para administrar dispositivos Intune de manera remota</span><span class="sxs-lookup"><span data-stu-id="89adf-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="89adf-103">Los dispositivos administrados por Intune se pueden administrar de forma remota con [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="89adf-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="89adf-104">Para administrar Intune con TeamViewer, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="89adf-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="89adf-105">Empiece por obtener credenciales de TeamViewer para configurar el conector de TeamViewer en Intune.</span><span class="sxs-lookup"><span data-stu-id="89adf-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="89adf-106">Esto permite que el administrador introduzca las credenciales en la interfaz de usuario del conector de TeamViewer en Dispositivos, una operación única para establecer el vínculo entre Intune y el servicio TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="89adf-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="89adf-107">**Parte 1: iniciar una sesión con un dispositivo remoto**</span><span class="sxs-lookup"><span data-stu-id="89adf-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="89adf-108">En **Todos los dispositivos**, seleccione el dispositivo en el que desea iniciar una sesión remota.</span><span class="sxs-lookup"><span data-stu-id="89adf-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="89adf-109">En **... Más**, seleccione **Nueva sesión de asistencia remota**.</span><span class="sxs-lookup"><span data-stu-id="89adf-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="89adf-110">Seleccione **Sí** para confirmar que desea establecer una sesión remota.</span><span class="sxs-lookup"><span data-stu-id="89adf-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="89adf-111">Después de que el servicio TeamViewer reconozca la solicitud "Inicio de una nueva sesión remota", verá una opción para **Iniciar asistencia remota** en los detalles del panel de Información general (o en Essentials) del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89adf-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="89adf-112">Seleccione **Ver más** para expandir el panel y mostrar el estado de Asistencia remota.</span><span class="sxs-lookup"><span data-stu-id="89adf-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="89adf-113">Seleccione **Iniciar sesión remota** para iniciar la sesión en el lado del administrador.</span><span class="sxs-lookup"><span data-stu-id="89adf-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="89adf-114">Elija descargar el binario de TeamViewer (Windows) y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="89adf-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="89adf-115">**Nota** Puede ignorar cualquier página de explorador web abierta en el sitio web de TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="89adf-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="89adf-116">Acepte la solicitud para que la aplicación de TeamViewer realice cambios en el dispositivo (solo Windows).</span><span class="sxs-lookup"><span data-stu-id="89adf-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="89adf-117">Se inicia la aplicación de TeamViewer y se incluye el código de la sesión para autenticar la conexión con el dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="89adf-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="89adf-118">**Parte 2: dispositivo destino de una sesión remota**</span><span class="sxs-lookup"><span data-stu-id="89adf-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="89adf-119">Abra el portal de la empresa de Intune.</span><span class="sxs-lookup"><span data-stu-id="89adf-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="89adf-120">Busque la marca de notificación: "Su administrador de TI solicita el control de este dispositivo para una sesión de asistencia remota" y seleccione la notificación.</span><span class="sxs-lookup"><span data-stu-id="89adf-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="89adf-121">Elija descargar la aplicación de TeamViewer o confirme la descarga de la aplicación de TeamViewer desde el App Store y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="89adf-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="89adf-122">**Nota** Puede ignorar cualquier página de explorador web abierta en el sitio web de TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="89adf-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="89adf-123">Acepte la solicitud para que la aplicación de TeamViewer realice cambios en el dispositivo (solo Windows).</span><span class="sxs-lookup"><span data-stu-id="89adf-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="89adf-124">Se inicia la aplicación de TeamViewer y se incluye el código de la sesión para autenticar la conexión con el dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="89adf-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="89adf-125">Se le preguntará si desea permitir el inicio de la sesión.</span><span class="sxs-lookup"><span data-stu-id="89adf-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="89adf-126">**Nota** Los códigos de sesión generados por el servicio TeamViewer son de uso único.</span><span class="sxs-lookup"><span data-stu-id="89adf-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="89adf-127">Si pierde la conexión, debe:</span><span class="sxs-lookup"><span data-stu-id="89adf-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="89adf-128">Cerrar la instancia de la aplicación de TeamViewer en el dispositivo remoto y en la estación de trabajo de administración.</span><span class="sxs-lookup"><span data-stu-id="89adf-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="89adf-129">Cerrar el portal de la empresa en el dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="89adf-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="89adf-130">Iniciar una nueva "Nueva sesión de asistencia remota" en el portal de administración.</span><span class="sxs-lookup"><span data-stu-id="89adf-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="89adf-131">Volver a abrir el portal de la empresa en el dispositivo remoto para recibir la nueva notificación.</span><span class="sxs-lookup"><span data-stu-id="89adf-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="89adf-132">Descargar y abrir la aplicación de TeamViewer en el dispositivo remoto y en la estación de trabajo de administración, como antes.</span><span class="sxs-lookup"><span data-stu-id="89adf-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>