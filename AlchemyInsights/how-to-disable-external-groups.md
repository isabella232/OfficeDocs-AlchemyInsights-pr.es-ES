---
title: Cómo deshabilitar grupos externos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015637"
---
# <a name="how-to-disable-external-groups"></a>Cómo deshabilitar grupos externos

Yammer mensajería externa aplica Exchange de transporte (ETR), un conjunto de controles proactivos para evitar que se comparta la información de la empresa. Para restringir a los usuarios la creación de grupos externos, debe configurar una regla de transporte de Exchange (ETR) y, a continuación, configurar Yammer para usar la regla de transporte de Exchange para bloquear la mensajería externa.
  
Una vez que haya creado una regla en el Exchange Online de administración, siga estos pasos para establecer ETR para que se aplique en Yammer:
  
- Inicie sesión en Yammer como administrador comprobado y, en el Centro de administración de **Yammer,** vaya a C **Content and Security Security \> Configuración.**

- En **Mensajería externa,** seleccione Aplicar las Exchange Online Exchange de transporte **(ETR) en Yammer.**

- Seleccione **Guardar**.

Para obtener más información, vea [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  