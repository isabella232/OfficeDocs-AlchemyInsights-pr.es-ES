---
title: Solucionar problemas al iniciar sesión en OneDrive
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8283"
- "9004614"
ms.openlocfilehash: fb944ae8dac7a8a222d2946025d8009216d6ca02efa750977bc9037bf578c8a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972625"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a>Solucionar problemas al iniciar sesión en OneDrive

En este artículo se describen las siguientes situaciones:

- Solución de problemas al iniciar sesión en el cliente de sincronización de OneDrive
- Solución de problemas al iniciar sesión en el sitio de OneDrive para la Empresa

**Solución de problemas al iniciar sesión en el cliente de sincronización de OneDrive**

- Para ver los pasos para el error 0x004de40, consulte [Código de error 0x8004de40 al iniciar sesión en OneDrive](/sharepoint/troubleshoot/administration/error-0x8004de40-in-onedrive).
- Inicie sesión en el sitio de OneDrive o SharePoint. Para ello, visite el sitio y haga clic en el botón **Sincronizar** de la parte superior de la barra de menús del sitio.
- Asegúrese de iniciar sesión en OneDrive para la Empresa y no en OneDrive.com. Si la dirección URL que visita empieza por onedrive.live.com, entonces no es la ubicación de su OneDrive para la Empresa. Una forma sencilla de asegurarse de que inicia sesión en OneDrive para la Empresa es seguir este vínculo https://portal.office.com/onedrive y usar su cuenta profesional o educativa para iniciar sesión.
- Si todavía tiene problemas, considere la posibilidad de [restablecer OneDrive](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c).
- [Desvincule la cuenta de OneDrive](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1), inicie sesión en el sitio de OneDrive o SharePoint y, después, haga clic en el botón **Sincronizar** de la parte superior de la barra de menús del sitio.

**Solución de problemas al iniciar sesión en el sitio de OneDrive para la Empresa**

- Asegúrese de iniciar sesión en OneDrive para la Empresa y no en OneDrive.com. Si la dirección URL que visita empieza por onedrive.live.com, entonces no es la ubicación de su OneDrive para la Empresa. Una forma sencilla de asegurarse de que inicia sesión en OneDrive para la Empresa es seguir este vínculo https://portal.office.com/onedrive y usar su cuenta profesional o educativa para iniciar sesión.
- Si se le redirige a la página de perfil de Delve, un administrador de Microsoft 365 deberá [conceder a los usuarios el derecho de crear su sitio de OneDrive para la Empresa](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0).
- Compruebe que puede visitar el sitio de OneDrive con [Exploración de InPrivate en Microsoft Edge](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc) (o una característica similar en otro explorador).
    - Si la Exploración de InPrivate funciona, es posible que deba [borrar los datos de exploración en Microsoft Edge](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4) (o una característica similar en otro explorador).

**Solución de problemas al iniciar sesión en Office para sincronizar con OneDrive**

Si recibe alguno de los siguientes mensajes de error: **Carga bloqueada**, **Iniciar sesión para guardar este archivo** o **Guardar una copia**, es posible que deba [quitar y reconectar OneDrive desde sus servicios conectados de Office](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8).

**Otras recomendaciones para la solución de problemas**

Si es administrador global, de licencia o de usuario, [asigne la licencia correcta a los usuarios afectados](/microsoft-365/admin/manage/assign-licenses-to-users).

