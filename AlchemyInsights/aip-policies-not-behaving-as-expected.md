---
title: 'AIP: las directivas no se comportan como se esperaba'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934310"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: las directivas no se comportan como se esperaba

Azure Information Protection: las directivas no se comportan como se esperaba. Consulte el texto a continuación para obtener instrucciones recomendadas para diferentes aspectos de directiva:

1. Si tiene problemas con las marcas visuales, consulte [Cuando se aplican marcas visuales](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Si tiene problemas con el etiquetado automático, consulte [Cómo configurar las condiciones de la clasificación automática y recomendada para Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) y [¿Qué intentan detectar los tipos de información confidencial?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Si tiene problemas con la protección Nativa/Pfile, consulte [Configuración de la API de archivo](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Compruebe si usa directivas de ámbito que no están correctamente configuradas: [Cómo configurar la directiva de Azure Information Protection para determinados usuarios al usar las directivas de ámbito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Si el etiquetado automático no funciona para Outlook cuando se adjunte un documento etiquetado, compruebe que DRMEncryptProperty no se ha definido como se describe a continuación: [Configuración del registro de IRM para seguridad](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Si sigue experimentando problemas, recopile los registros de los clientes de Azure Information Protection y adjunte los registros exportados a este vale.

1. Abra un documento de Office o cree un nuevo correo electrónico en Outlook.
2. Haga clic en **Proteger/Confidencialidad** > **Ayuda y comentarios**.
3. Haga clic en **Exportar registros**.
4. Guarde los registros en la ubicación que desee y adjúntelos a esta solicitud de servicio.

Recursos adicionales:

- [Cómo configurar una etiqueta para las marcas visuales de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Revisar la documentación de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Usar las etiquetas de confidencialidad en Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

