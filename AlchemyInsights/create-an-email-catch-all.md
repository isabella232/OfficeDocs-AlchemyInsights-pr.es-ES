---
title: Crear un correo electrónico capturar todo
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816217"
---
# <a name="create-an-email-catch-all"></a>Crear un correo electrónico capturar todo

El uso de una captura de todo está muy desaconsejado. Es mejor proporcionar un rebote al remitente que le permite a los remitentes saber que su mensaje no se pudo entregar como se ha dirigido para que puedan tomar medidas. También puede limitar el buzón supervisado para que solo pueda capturar direcciones de correo electrónico que antes eran válidas. 

Cualquier buzón de correo catch recibirá una gran cantidad de correo no deseado y, finalmente, puede rellenarse si no se supervisa de cerca. (Hay límites de recepción). 

Si decide continuar, siga estos pasos:

1. Crear un grupo de distribución dinámico & incluir "Todos los tipos de destinatarios".

2. Cree un buzón dedicado para capturar correos electrónicos, por ejemplo, catchall@domain.com.

3. Para el dominio específico, establezca DomainType en "InternalRelay". Si más adelante quita la captura de todo, asegúrese de volver a establecer el dominio en Autoritativo.

4. Cree una regla de transporte de flujo de correo de la siguiente manera:

    - Si el remitente es "Fuera de la organización"
    - Redirigir el mensaje a Catchall@domain.com
    - Excepto si el destinatario es miembro de allusers@domain.com (el grupo de distribución contiene todos los miembros)
    - Asegúrese de validar que los nuevos buzones se agregan al grupo de distribución dinámica
