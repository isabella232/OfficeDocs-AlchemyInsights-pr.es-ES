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
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Limpieza automática de dispositivos obsoletos en Intune

Intune permite que el administrador configure un intervalo de tiempo entre 90 y 270 días, tras el cual se eliminan los dispositivos obsoletos del servicio. Esta configuración se aplica a toda la organización y, una vez activada, tiene efecto de forma inmediata. Los dispositivos que no han sido revisados en el servidor de Intune durante un período superior al configurado se eliminan de forma permanente.

**Nota** Solo los objetos de dispositivos MDM son aptos para esta acción de limpieza. Solo se excluyen los objetos de dispositivo EAS.

Para obtener información adicional sobre cuándo un dispositivo se convierte en apto para su eliminación sobre la base de la configuración de limpieza del dispositivo y su "estado":

Configuración: **Eliminar dispositivos después de la última fecha de registro: Sí (un valor (N) en días especificados)**

- Sobre la base del valor (N) establecido en la configuración, el servicio de Intune elimina el dispositivo en los días especificados una vez que se haya registrado con éxito por última vez.

Configuración: **Eliminar dispositivos después de la última fecha de registro: No**

- 180 días después de el certificado del dispositivo expire y no se renueve, el dispositivo se elimina.

**Nota** En ambos casos, el dispositivo se debe registrar de forma correcta en Intune. El registro se lleva a cabo durante el primer registro del dispositivo con el servicio Intune.

Si un dispositivo se inscribe de forma correcta en Intune, pero no se registra en este servicio, el dispositivo se elimina 270 días después de la inscripción. (90 días para marcar el dispositivo como revocado y luego otros 180 días para eliminar el registro).

Actualmente, no existe ningún mecanismo en la consola de Intune para establecer la fecha de expiración de la certificación del dispositivo para un dispositivo determinado.