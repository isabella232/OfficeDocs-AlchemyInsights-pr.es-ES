---
title: Corregir problemas comunes con Microsoft Defender para Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330077"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Corregir problemas comunes con Microsoft Defender para Office 365

Estas son algunas soluciones a problemas comunes con Microsoft Defender para Office 365:

- **Retraso del mensaje:**

  Los retrasos en la entrega de correo electrónico pueden deberse Caja fuerte datos adjuntos de análisis de mensajes. Para obtener más información, [vea Caja fuerte configuración de directiva de datos adjuntos](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Informe de resultados falsos positivos o negativos:**

  Para obtener más información, consulte [Notificar mensajes y archivos a Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Habilitar Caja fuerte de vínculos**:

  1. En el portal Microsoft 365 Defender en , vaya a Correo electrónico & directivas de colaboración & reglas de amenazas Caja fuerte vínculos en la <https://security.microsoft.com/>  \>  \>  \>  **sección** Directivas.

     Para ir directamente a la **página Caja fuerte vínculos,** use <https://security.microsoft.com/safelinksv2> .

  2. En la **Caja fuerte vínculos,** seleccione la directiva haciendo clic en el nombre de la directiva.
  3. En el menú desplegable de detalles que aparece, realice uno de los pasos siguientes:
     - Para agregar una nueva directiva, seleccione **+ Crear**. Se iniciará un asistente para ayudarle a definir la configuración de la directiva.
     - Para editar una directiva existente, seleccione la directiva haciendo clic en el nombre de la directiva. En el control desplegable de detalles que aparece, seleccione **Editar en** la sección **Configuración de** protección.
  4. En la **página Configuración de** protección, configure las siguientes opciones:
     - Activar Seleccione la acción para direcciones URL **potencialmente malintencionadas desconocidas en los mensajes**.
     - Seleccione **Aplicar vínculos seguros a los mensajes enviados dentro de la organización**.

  Para obtener más información, vea [Configurar directivas Caja fuerte vínculos en Microsoft Defender para Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
