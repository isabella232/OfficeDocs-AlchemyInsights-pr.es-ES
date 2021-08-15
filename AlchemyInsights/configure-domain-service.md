---
title: Configurar el servicio de dominio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: cf8ea7d73adf36f71ae92abad48ef9b664eb0c96094a38750c86cf42958b5323
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994782"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>No se puede habilitar AAD-DS o la implementación falla

Para resolver el problema por el que Azure AD Domain Services (AAD-DS) no se habilita o no se implementa correctamente, realice los pasos siguientes:

1. Si usa una red virtual ya existente, busque en su NSG reglas que bloquean puertos necesarios para sincronizar con AAD-DS en el portal https://aka.ms/aadds-networking.
2. Compruebe si hay una respuesta para el mensaje de error en esta guía de solución de problemas que está disponible en https://aka.ms/aadds-troubleshoot-enable.
3. Pruebe a implementar Azure AD Domain Services en una nueva red virtual.
4. Siga la guía de Introducción sobre cómo implementar AAD-DS: [Crear y configurar los Servicios de dominio de AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Si tiene problemas con la implementación de Azure AD Domain Services, consulte [Solución de problemas de Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) para resolver errores comunes y obtener ayuda para restaurar el funcionamiento. 

**No se puede deshabilitar AAD-DS**

AAD-DS no se puede pausar. Si quiere dejar de usar el dominio administrado, debe eliminarlo.
Para eliminar el dominio administrado, vea [Eliminar AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



