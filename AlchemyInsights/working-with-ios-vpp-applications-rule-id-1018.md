---
title: Trabajar con iOS VPP Applications Rule Id. 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083031"
---
# <a name="working-with-ios-vpp-applications"></a>Trabajar con aplicaciones VPP de iOS

Lee Cómo administrar las aplicaciones [de iOS](https://docs.microsoft.com/intune/vpp-apps-ios) compradas a través de un programa de compra por volumen con Microsoft Intune para obtener información sobre características, restricciones y pasos para usar el Programa de compras por volumen de Apple y la compatibilidad con él en Microsoft Intune.
  
 **Problemas comunes:** "Asigné una aplicación VPP de iOS a mis usuarios, pero la instalación no se pudo hacer".
  
- Esto puede ocurrir si se usa un único token VPP en varios proveedores de administración de dispositivos móviles. Los tokens VPP de Apple solo se pueden usar con un proveedor. Si usó un token VPP con varios proveedores, debe volver a cargar el token en Intune.

- La instalación también puede producir errores si el número total de instalaciones supera el número de licencias. Para ver un informe de uso de las licencias, vaya a la página Licencias de aplicaciones **móviles** \> **de** Intune. Para obtener información sobre cómo recuperar licencias en uso, consulte [este artículo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
