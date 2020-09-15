---
title: Código de error 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Si recibe un error al activar Office 2013 en implementaciones de servicios de escritorio remoto (RDS), considere la posibilidad de habilitar ADAL editando el registro.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709204"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Error al activar Office 2013 en servicios de escritorio remoto

Si recibe un error al activar Office 2013 en implementaciones de servicios de escritorio remoto (RDS), considere la posibilidad de habilitar ADAL editando el registro.
  
|**Clave del registro**|**Tipo**|**Valor**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

Para obtener más información, consulte [Habilitar la autenticación moderna para Office 2013 en dispositivos Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL está habilitado de forma predeterminada en las aplicaciones de Microsoft 365 para empresas y Office 2016. Servicios de escritorio remoto (RDS) se llamaba Terminal Services.
  