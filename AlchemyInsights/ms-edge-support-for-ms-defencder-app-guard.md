---
title: Soporte de Microsoft Edge para la protección de aplicaciones de Microsoft defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576635"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Soporte de Microsoft Edge para la protección de aplicaciones de Microsoft defender

Diseñada para Windows 10 y Microsoft Edge, la protección de aplicaciones usa un enfoque de aislamiento de hardware que permite a un usuario navegar por un sitio que no es de confianza desde dentro de un contenedor aislado, compatible con Hyper-V, separado del sistema operativo host.

Un administrador de la empresa define una lista de sitios web de confianza, recursos de la nube y redes internas. Cuando un usuario visita un sitio que no se encuentra en la lista, Microsoft Edge abrirá el sitio en el contenedor. Esto significa que si el sitio resulta ser malintencionado, el equipo host seguirá protegido y el atacante no recibirá los datos de la empresa.

La instalación de extensiones en el contenedor es compatible con la versión 81 de Microsoft Edge y puede controlarse a través de una directiva. La dirección updateURL que se usa en la Directiva ExtensionInstallForcelist debe agregarse como un recurso neutro en las directivas de aislamiento de red que usa la protección de aplicaciones.

Para obtener más información, vea [compatibilidad de Microsoft Edge con protección de aplicaciones de Microsoft defender](https://go.microsoft.com/fwlink/?linkid=2134229).
