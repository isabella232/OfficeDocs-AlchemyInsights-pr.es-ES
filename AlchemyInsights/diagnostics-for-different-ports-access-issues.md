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
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnósticos de problemas de acceso a diferentes puertos

Para resolver los problemas de acceso a diferentes puertos, realice los pasos siguientes:

1. Detenga o desasigne la máquina virtual (VM) desde el portal, reiníciela y vuelva a probar. 
2. Compruebe la configuración de red de la máquina virtual para determinar si hay grupos de seguridad de red (NSG) que están bloqueando el tráfico. También puede usar la [Herramienta de comprobación del flujo de IP de Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) para comprobar si hay NSG que bloquean el tráfico, rutas definidas por el usuario (UDR) que están volviendo a dirigir el tráfico al entorno local ("Ruta predeterminada" 0.0.0.0/0) o a un aparato de red.
Si sigue teniendo problemas después de probar los pasos anteriores, proporcione el nombre de la máquina virtual y el puerto TCP en el que está intentando enviar el correo para un mejor diagnóstico.

**Documentos recomendados**

[Limitaciones y recomendaciones para enviar el correo electrónico saliente a través del puerto 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)