---
title: Limpieza automática de dispositivos obsoletos en Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505234"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="33924-102">Limpieza automática de dispositivos obsoletos en Intune</span><span class="sxs-lookup"><span data-stu-id="33924-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="33924-103">Intune permite que el administrador configure un intervalo de tiempo entre 90 y 270 días, tras el cual se eliminan los dispositivos obsoletos del servicio.</span><span class="sxs-lookup"><span data-stu-id="33924-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="33924-104">Esta configuración se aplica a toda la organización y, una vez activada, tiene efecto de forma inmediata.</span><span class="sxs-lookup"><span data-stu-id="33924-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="33924-105">Los dispositivos que no han sido revisados en el servidor de Intune durante un período superior al configurado se eliminan de forma permanente.</span><span class="sxs-lookup"><span data-stu-id="33924-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="33924-106">**Nota** Solo los objetos de dispositivos MDM son aptos para esta acción de limpieza.</span><span class="sxs-lookup"><span data-stu-id="33924-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="33924-107">Solo se excluyen los objetos de dispositivo EAS.</span><span class="sxs-lookup"><span data-stu-id="33924-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="33924-108">Para obtener información adicional sobre cuándo un dispositivo se convierte en apto para su eliminación sobre la base de la configuración de limpieza del dispositivo y su "estado":</span><span class="sxs-lookup"><span data-stu-id="33924-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="33924-109">Configuración: **Eliminar dispositivos después de la última fecha de registro: Sí (un valor (N) en días especificados)**</span><span class="sxs-lookup"><span data-stu-id="33924-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="33924-110">Sobre la base del valor (N) establecido en la configuración, el servicio de Intune elimina el dispositivo en los días especificados una vez que se haya registrado con éxito por última vez.</span><span class="sxs-lookup"><span data-stu-id="33924-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="33924-111">Configuración: **Eliminar dispositivos después de la última fecha de registro: No**</span><span class="sxs-lookup"><span data-stu-id="33924-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="33924-112">180 días después de el certificado del dispositivo expire y no se renueve, el dispositivo se elimina.</span><span class="sxs-lookup"><span data-stu-id="33924-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="33924-113">**Nota** En ambos casos, el dispositivo se debe registrar de forma correcta en Intune.</span><span class="sxs-lookup"><span data-stu-id="33924-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="33924-114">El registro se lleva a cabo durante el primer registro del dispositivo con el servicio Intune.</span><span class="sxs-lookup"><span data-stu-id="33924-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="33924-115">Si un dispositivo se inscribe de forma correcta en Intune, pero no se registra en este servicio, el dispositivo se elimina 270 días después de la inscripción.</span><span class="sxs-lookup"><span data-stu-id="33924-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="33924-116">(90 días para marcar el dispositivo como revocado y luego otros 180 días para eliminar el registro).</span><span class="sxs-lookup"><span data-stu-id="33924-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="33924-117">Actualmente, no existe ningún mecanismo en la consola de Intune para establecer la fecha de expiración de la certificación del dispositivo para un dispositivo determinado.</span><span class="sxs-lookup"><span data-stu-id="33924-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>