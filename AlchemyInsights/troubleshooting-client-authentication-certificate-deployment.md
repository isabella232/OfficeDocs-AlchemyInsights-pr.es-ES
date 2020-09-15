---
title: Solución de problemas de implementación de certificados de autenticación de cliente
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659003"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Solución de problemas de implementación de certificados de autenticación de cliente

Los perfiles de certificados de cliente de Intune NDES/SCEP y PKCS/PFX suelen usarse en combinación con otros tipos de perfiles, como WiFi, VPN y correo electrónico, para permitir que los usuarios puedan autenticarse en los recursos corporativos. Cuando estos tipos de perfil están vinculados a un perfil de certificado de cliente dependen de la implementación correcta de este perfil.

La configuración inicial de la infraestructura y la configuración asociada del perfil de certificado del cliente a menudo necesitan solucionar un problema. Para obtener una guía paso a paso para configurar correctamente el conector NDES y las instrucciones para la solución de problemas para aislar problemas con la implementación de certificados, vea: 

- [Configurar la infraestructura de para admitir SCEP con Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Información general sobre la solución de problemas de perfiles de certificado SCEP con Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

Use los scripts de PowerShell a los que se hace referencia para ayudar a comprobar la configuración. Para obtener más información, consulte [Scripts de Verificación de conectores de Certificados de Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Otros problemas comunes**

**Cuando intento instalar el conector de certificados de Intune en el servidor de conectores de NDES, recibo el mensaje "no se puede comprobar la contraseña de la solicitud de certificado". Es posible que ya se haya usado. Obtenga una nueva contraseña para enviar con esta solicitud ".**  

Este mensaje quiere decir que debe ejecutar la instalación de conector de certificados como administrador.

En algunos entornos, los servidores en los que se ejecuta el certificado de Intune deben usar un servidor proxy para conectarse a Intune y, por lo tanto, el conector de certificados debe usar un proxy. En algunos casos, NDES Connector omite la configuración de proxy configurada y puede que sea necesario configurar la configuración de proxy mientras se ejecuta en el contexto de seguridad de LocalSystem. 
 
La solución consiste en ejecutar Internet Explorer como SYSTEM y configurar un servidor proxy en IE. Después de reiniciar el servicio del conector Intune, el conector NDES se conecta a Intune.

**Los dispositivos de los usuarios ya no reciben certificados SCEP de NDES.**

Es posible que el certificado de autenticación de cliente emitido al servidor NDES y que se especifica durante la instalación de NDES Connector, haya expirado o no se encuentra. Para resolver: 
 
1. Desinstale el conector NDES.  
2. Use estos detalles para solicitar una nueva autenticación de cliente o certificado de autenticación de servidor: 
 
    - Nombre de firmante: CN=FQDN externo  
    - Nombre alternativo del firmante (se requieren ambos): DNS = FQDN externo, DNS=FQDN interno 
 
3. Vuelva a instalar el conector NDES con el nuevo certificado.