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
description: Si recibe un error al activar Office 2013 en implementaciones de Servicios de Escritorio remoto (RDS), considere la posibilidad de habilitar ADAL editando el Registro.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316703"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Error al activar Office 2013 en Servicios de Escritorio remoto

Si recibe un error al activar Office 2013 en implementaciones de Servicios de Escritorio remoto (RDS), considere la posibilidad de habilitar ADAL editando el Registro.
  
|**Clave del registro**|**Tipo**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

Para obtener más información, vea [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
**Nota:** ADAL está habilitado de forma predeterminada en Aplicaciones Microsoft 365 para empresas y Office 2016. Servicios de Escritorio remoto (RDS) se denominaba anteriormente Terminal Services.
  