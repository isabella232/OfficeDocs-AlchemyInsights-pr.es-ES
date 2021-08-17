---
title: Conjunto de réplicas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110697"
---
# <a name="replica-set"></a>Conjunto de réplicas

AADDS también se llama como dominio administrado. En realidad, el back-end ejecuta y mantiene dos controladores de dominio. Los dos DC incluyen un CONTROLADOR de dominio principal y un CONTROLADOR de dominio de replicación. Las copias de seguridad en AADDS (dominio administrado) son un proceso automatizado administrado por la plataforma de Azure. En caso de que se produce un problema con el dominio administrado, el soporte técnico de Azure puede ayudarle a restaurar desde la copia de seguridad.

Cada conjunto de réplicas se crea en una red virtual. Cada red virtual debe estar emparejada con todas las demás redes virtuales que hospedan el conjunto de réplicas de un dominio administrado. Esta configuración crea una topología de red de malla que admite la replicación de directorios. Una red virtual puede admitir varios conjuntos de réplicas, siempre que cada conjunto de réplicas esté en una subred virtual diferente.

Para obtener más información sobre el conjunto de réplicas, vea [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
