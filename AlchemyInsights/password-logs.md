---
title: Registros de contraseñas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960960"
---
# <a name="password-logs"></a>Registros de contraseñas

**Tengo problemas al acceder a los registros de auditoría del restablecimiento de contraseña**

Para solucionar los problemas relacionados con el acceso a los registros de auditoría del restablecimiento de contraseña, realice el siguiente paso:

Asegúrese de que está autorizado para ver los registros de auditoría. 

Solo se autorizan los roles siguientes:
 - Administrador global
 - Administrador de seguridad
 - Lector de seguridad

**Quiero ver todos los eventos de auditoría del restablecimiento de contraseñas desde el momento de la implementación inicial**

Se almacenan hasta 120 000 eventos de restablecimiento o registro de contraseñas en los informes de los últimos 30 días. Este límite máximo se aplica a la interfaz de usuario al descargar el archivo CSV. Hay disponibles 1 millón de eventos a través de PowerShell.
Para más información, vea los vínculos siguientes:

- [Eventos de restablecimiento de contraseña de autoservicio desde Azure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cómo descargar rápidamente eventos de registro de restablecimiento de contraseña con PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Quiero obtener más información sobre las funcionalidades de informes de restablecimiento de contraseñas**

Compruebe quién se registra o restablece contraseñas con los registros de auditoría de restablecimiento de contraseña de Azure AD en Azure Portal en **Usuarios y grupos**.
Para más información, consulte los siguientes vínculos:

- [Información general sobre los informes de restablecimiento de contraseña](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cómo ver los informes de restablecimiento de contraseña en Azure Portal](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Eventos de restablecimiento de contraseña de autoservicio desde Azure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Cómo descargar rápidamente eventos de registro de restablecimiento de contraseña con PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


