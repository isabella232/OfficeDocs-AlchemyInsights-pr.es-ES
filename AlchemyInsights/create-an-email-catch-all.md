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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080763"
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
