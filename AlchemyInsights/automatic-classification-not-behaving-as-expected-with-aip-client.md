---
title: La clasificación automática no se comporta de la forma esperada con el cliente de AIP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715218"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>La clasificación automática no se comporta de la forma esperada con el cliente de AIP

La clasificación automática no se comporta como se esperaba. Use las siguientes instrucciones recomendadas:

1. Si tiene problemas con el etiquetado automático, consulte [Cómo configurar las condiciones de la clasificación automática y recomendada para Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) y [¿Qué intentan detectar los tipos de información confidencial?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Compruebe si usa directivas de ámbito que no están correctamente configuradas: [Cómo configurar la directiva de Azure Information Protection para determinados usuarios al usar las directivas de ámbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Si el etiquetado automático no funciona para Outlook cuando se adjunte un documento etiquetado, compruebe que `DRMEncryptProperty` no se ha definido como se describe a continuación: [Configuración del registro de IRM para seguridad.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Si ha usado los [tipos de información integrada](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) para su directiva de Azure Information Protection, compruebe que el contenido coincida con el formato esperado.
5. Compruebe que la etiqueta está configurada de forma adecuada para **Automático** o **Recomendado**. La etiqueta **Automática** está disponible para todas las aplicaciones de Microsoft 365, mientras que **Recomendado** está disponible para todas las aplicaciones de Microsoft 365 salvo Outlook.
6. No puede usar la clasificación automática para documentos y mensajes de correo electrónico que se etiquetaran previamente, ya sea de forma manual o automática, con una clasificación más alta.  Para más información, consulte: [Forma de aplicar etiquetas recomendadas o automáticas](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Si sigue experimentando problemas, recopile los registros de los clientes de Azure Information Protection y adjunte los registros exportados a este vale de soporte. Para exportar documentos de Azure Information Protection:
    - Abra un documento de Office o cree un nuevo correo electrónico en Outlook.
    - Haga clic en **Proteger/Confidencialidad** > **Ayuda y comentarios**.
    - Haga clic en **Exportar registros**.
    - Guarde los registros en la ubicación que desee y adjúntelos a su solicitud de servicio.

Para obtener más información, consulte:

- [Cómo configurar condiciones para la clasificación automática y recomendada para Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Guías de procedimientos para situaciones comunes que usan Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Revisar la documentación de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Revisar las características y suscripciones de Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Requisitos de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).
- [Tutorial rápido para Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).
- [Descargar el cliente de Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
