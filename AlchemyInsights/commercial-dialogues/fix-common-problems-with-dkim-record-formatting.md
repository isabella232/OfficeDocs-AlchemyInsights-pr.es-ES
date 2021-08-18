---
title: Corregir problemas comunes con el formato de registro DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324007"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Corregir problemas comunes con el formato de registro DKIM

La mayoría de los problemas de configuración dkim están relacionados con registros DNS incorrectos.

Para corregir los problemas de configuración de DKIM, compruebe que el registro DKIM CNAME **(no** un registro TXT) tiene el formato correcto. Para obtener más información, vea [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Si necesita ayuda con registros DNS en general, vea [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

**Nota:** Después de crear o actualizar los registros DNS DKIM en el servicio de hospedaje DNS de su dominio, tendrá que esperar a que se propaguen los registros DNS.
