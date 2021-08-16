---
title: Configuración de red virtual con Azure AD Domain Services
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
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072861"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Configuración de red virtual con Azure AD Domain Services

Siga los siguientes pasos para realizar la configuración de red virtual con Azure AD Domain Services: 

1. Compruebe el estado de su dominio en el Azure Portal https://aka.ms/aadds-health
2. Compruebe si su NSG contiene reglas que bloqueen los puertos necesarios para la sincronización en Azure Active Directory Domain Services que estén en el portalhttps://aka.ms/aadds-networking
3. Asegúrese de que su red virtual esté implementada en la misma región de Azure que su dominio administrado de Azure AD Domain Services.
4. Asegúrese de que no tiene ningún dominio con el mismo nombre de dominio disponible en la red virtual.

Para obtener más información sobre consideraciones de diseño de la red virtual de Azure compatibles con Azure AD Domain Services, consulte [Consideraciones sobre la red virtual](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

