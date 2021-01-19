---
title: 'Controlador de dominio '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886901"
---
# <a name="domain-controller"></a>Controlador de dominio

**No se puede habilitar AAD-DS o la implementación falla**

Para resolver el problema por el que Azure AD Domain Services (AAD-DS) no se habilita o no se implementa correctamente, realice los pasos siguientes:

1. Si usa una red virtual ya existente, busque en su NSG reglas que bloquean puertos necesarios para sincronizar con AAD-DS en el portal https://aka.ms/aadds-networking.
2. Compruebe si hay una respuesta para el mensaje de error en esta guía de solución de problemas que está disponible en https://aka.ms/aadds-troubleshoot-enable.
3. Pruebe a implementar Azure AD Domain Services en una nueva red virtual.
4. Siga la guía de Introducción sobre cómo implementar AAD-DS que está disponible en [Tutorial para crear Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Si tiene problemas con la implementación de Azure AD Domain Services, consulte [Solución de problemas de Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) para resolver errores comunes y obtener ayuda para restaurar el funcionamiento. 

**No se puede deshabilitar AAD-DS**

AAD-DS no se puede pausar. Si quiere dejar de usar el dominio administrado, debe eliminarlo.

Si tiene problemas, para resolver mensajes de error comunes y para conocer los pasos de solución de problemas asociados que le ayudarán a que todo vuelva a funcionar, consulte [Solución de problemas de Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
