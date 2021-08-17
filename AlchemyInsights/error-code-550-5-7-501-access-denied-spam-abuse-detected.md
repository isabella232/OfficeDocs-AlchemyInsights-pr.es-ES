---
title: Código de error 550 5.7.501 Access denied, spam abuse detected
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: a3eebe4e9d69e100a750e74a6d34ec67dc0566df5dd6eb59809adb07ed8a682f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044285"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Access denied, spam abuse detected

Normalmente, este mensaje se produce cuando los usuarios envían mensajes de correo electrónico desde direcciones IP mediante el dominio *inicial .onmicrosoft.com* asignado a nuevos inquilinos en Microsoft 365. La forma más sencilla de resolver este problema es:

1. [Agregue un dominio al espacio empresarial](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Cambie la dirección de correo electrónico principal de los usuarios](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) al nuevo dominio personalizado que acaba de agregar.
