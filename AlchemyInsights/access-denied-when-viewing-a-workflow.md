---
title: Acceso denegado al ver un flujo de trabajo
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955218"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acceso denegado al ver un flujo de trabajo

SharePoint flujos de trabajo de 2013 que intentan enviar un correo electrónico a un grupo de SharePoint pueden producir errores con un mensaje de error "Acceso denegado" si la pertenencia al grupo de SharePoint no está establecida en Todos.
  
 **Para resolver este problema, siga estos pasos:**
  
 1. Permitir que todos vean los miembros del SharePoint grupo.
  
 2. Quite el SharePoint de la línea Para o CC del correo electrónico.
  
 3. Agregue explícitamente los usuarios a la línea Para o CC si no se puede cambiar la visibilidad de pertenencia para SharePoint grupo.
  
Para ver más detalles, consulte [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  