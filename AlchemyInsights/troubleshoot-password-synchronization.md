---
title: Solucionar problemas de sincronización de contraseñas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105795"
---
# <a name="troubleshoot-password-synchronization"></a>Solucionar problemas de sincronización de contraseñas

Para solucionar problemas de sincronización de contraseñas, empiece por usar esta Conectar de solución de problemas de AAD para determinar por qué las contraseñas no se sincronizan. Para empezar, vaya a [Administrar sincronización directa](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Abra una nueva sesión Windows PowerShell sesión en el servidor Conectar Azure AD y seleccione **la opción Ejecutar como** administrador.

2. Ejecute Set-ExecutionPolicy RemoteSigned o Set-ExecutionPolicy Sin restricciones.

3. Inicie el Asistente para Conectar Azure AD.

4. Vaya a la página Tareas adicionales > **Solucionar**  >  **problemas siguientes**.

5. Seleccione **Iniciar** para abrir el menú solución de problemas de PowerShell.

6. Seleccione **Solucionar problemas de sincronización de contraseñas**.

    El problema suele ser que una contraseña no está sincronizada para una cuenta de usuario específica.

    **Notas** Se produce un error en la sincronización de contraseñas si la última sincronización correcta de contraseñas fue hace algún tiempo.

Para obtener más ayuda para solucionar problemas de sincronización de contraseñas, consulte [Troubleshoot password hash synchronization with Azure AD Conectar sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).