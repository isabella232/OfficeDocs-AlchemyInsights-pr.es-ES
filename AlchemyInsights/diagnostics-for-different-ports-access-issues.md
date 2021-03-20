---
title: Diagnósticos de problemas de acceso a diferentes puertos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897873"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="7df26-102">Diagnósticos de problemas de acceso a diferentes puertos</span><span class="sxs-lookup"><span data-stu-id="7df26-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="7df26-103">Para resolver los problemas de acceso a diferentes puertos, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="7df26-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="7df26-104">Detenga o desasigne la máquina virtual (VM) desde el portal, reiníciela y vuelva a probar.</span><span class="sxs-lookup"><span data-stu-id="7df26-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="7df26-105">Compruebe la configuración de red de la máquina virtual para determinar si hay grupos de seguridad de red (NSG) que están bloqueando el tráfico.</span><span class="sxs-lookup"><span data-stu-id="7df26-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="7df26-106">También puede usar la [Herramienta de comprobación del flujo de IP de Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) para comprobar si hay NSG que bloquean el tráfico, rutas definidas por el usuario (UDR) que están volviendo a dirigir el tráfico al entorno local ("Ruta predeterminada" 0.0.0.0/0) o a un aparato de red.</span><span class="sxs-lookup"><span data-stu-id="7df26-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="7df26-107">Si sigue teniendo problemas después de probar los pasos anteriores, proporcione el nombre de la máquina virtual y el puerto TCP en el que está intentando enviar el correo para un mejor diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="7df26-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="7df26-108">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="7df26-108">**Recommended Documents**</span></span>

[<span data-ttu-id="7df26-109">Limitaciones y recomendaciones para enviar el correo electrónico saliente a través del puerto 25</span><span class="sxs-lookup"><span data-stu-id="7df26-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)