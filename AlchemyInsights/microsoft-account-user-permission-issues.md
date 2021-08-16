---
title: 'Solución de problemas: usuario no encontrado en el directorio'
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098187"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Solución de problemas: usuario no encontrado en el directorio

Si los usuarios están recibiendo el mensaje de error "no se puede encontrar el usuario" en el directorio, vuelva a intentarlo donde el tipo de problema es Usuario no en el directorio.

Se pueden completar los siguientes pasos para solucionar el problema.

- Asegúrese de que la cuenta que aceptó la invitación de correo electrónico sea la misma cuenta que se usa para iniciar sesión más adelante. Asegúrese de que el usuario usa la misma cuenta para aceptar la invitación e iniciar sesión en el sitio. 

Para obtener más información, [consulta How to manage aliases for your Microsoft account to manage the Microsoft 365 </a> login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Vaya a cada sitio en el que el usuario recibe el error. 

Agregue "/_layouts/15/people.aspx/membershipgroupid=0" (dentro de las comillas dobles) al final de la dirección URL del sitio. 

Ejemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Seleccione el usuario de la lista.

- Haga **clic en Quitar permisos de usuario** de la cinta de opciones. 
-  Vuelva a agregar el usuario y vuelva a enviar la invitación al usuario.

