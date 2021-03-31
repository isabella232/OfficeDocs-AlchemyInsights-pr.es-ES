---
title: 126 ¿No se puede encontrar un error de obtención de un buzón en OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426679"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>¿No se encontró un error de buzón en Outlook en la web?

Si usa Outlook en la web y obtiene un buzón no se pudo encontrar por **error,** la cuenta que usó para conectarse a Outlook en la web no tiene una licencia de Exchange Online y, por lo tanto, no hay ningún buzón asociado a la cuenta. El administrador puede asignar una licencia a su cuenta siguiendo estos pasos:

1. Abra el [Centro de administración de Microsoft 365](https://portal.office.com/adminportal/home#/homepage) y vaya a **Usuarios** activos en la sección Usuarios y seleccione el usuario que ve el error. 

2. En la página de usuario  que se abre, vaya  a la sección Licencias y aplicaciones, seleccione el valor de ubicación adecuado y asigne una licencia que contenga Exchange Online (expanda la licencia para ver sus detalles). Cuando haya terminado, haga clic en **Guardar cambios**.

En algunos casos, si la licencia ya está asignada a una cuenta de usuario, quitar y reasignar la licencia ayuda a resolver el problema y a aprovisionar correctamente en el sistema: 

- Compruebe si sus suscripciones de M365 Exchange Online (y otras, si tiene alguna) están actualizadas y no han expirado recientemente.

Una vez que haya asegurado que la suscripción no ha expirado y que se ha asignado una licencia válida a la cuenta de usuario, la licencia puede tardar hasta 24 horas en aprovisionarse, por lo que es posible que tenga que esperar a que se resuelva el problema. Para obtener más información, consulta [Asignar y administrar licencias.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)