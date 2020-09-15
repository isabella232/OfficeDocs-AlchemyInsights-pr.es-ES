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
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688819"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acceso denegado al ver un flujo de trabajo

Los flujos de trabajo de SharePoint 2013 que intentan enviar un correo electrónico a un grupo de SharePoint pueden producir un error con un mensaje de error "acceso denegado" si la pertenencia del grupo de SharePoint no está establecida en todos.
  
 **Para solucionar este problema, siga estos pasos:**
  
 1. Permitir a todos los usuarios ver los miembros del grupo de SharePoint.
  
 2. Quite el grupo de SharePoint de la línea para o CC del correo electrónico.
  
 3. Agregue explícitamente los usuarios a la línea para o CC si no se puede cambiar la visibilidad de la pertenencia al grupo de SharePoint.
  
Para ver más detalles, consulte [http no autorizado a/_vti_bin/Client.SVC/SP.Utilities.Utility.sendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  