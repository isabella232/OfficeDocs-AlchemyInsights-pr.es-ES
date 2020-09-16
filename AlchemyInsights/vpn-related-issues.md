---
title: Problemas relacionados con la VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726108"
---
# <a name="vpn-related-issues"></a>Problemas relacionados con la VPN

La implementación correcta de conectividad VPN para los clientes MDM depende de un perfil implementado que refleja correctamente los requisitos de la infraestructura de VPN. Para ver la configuración adecuada para las plataformas cliente que está investigando, vea: 

[Configuración de dispositivos de Windows 10 y Windows Holographic para agregar conexiones VPN con Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Agregar una configuración de VPN en dispositivos iOS y iPad en Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Configuración de dispositivo Android para configurar VPN en Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Agregar la configuración de VPN en los dispositivos macOS en Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Si su perfil de VPN usa la autenticación basada en certificados, asegúrese de que el certificado raíz y los perfiles de certificación de autenticación de cliente vinculados al perfil de VPN se implementan correctamente.

**Problemas comunes**

**Desplegó un perfil de VPN en un dispositivo. Intune muestra que se completó correctamente, pero el dispositivo no se conecta a la VPN.**

Un estado correcto significa que Intune ha implementado correctamente el perfil como configurado. Sin embargo, estas configuraciones podrían no coincidir con los requisitos de red y/o autenticación. Revisar registros en el servicio de autenticación y infraestructura (en el servidor VPN y en el servidor NPS/RADIUS) para más información sobre el intento de conexión. Es posible que tenga que colaborar con el equipo de infraestructura de red o el proveedor de VPN de terceros para recopilar y revisar registros.

**Cuando configuro una VPN personalizada para iOS, la característica VPN por aplicación no está disponible.**

La VPN por aplicación para dispositivos iOS en Intune está actualmente disponible para una lista específica de proveedores y asociados, que también deben cumplir los requisitos previos de certificados antes de configurar una VPN por aplicación. Para obtener más información, consulte [Configurar la red privada virtual (VPN) de cada aplicación para dispositivos iOS/iPad en Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Para obtener más información acerca de todos los tipos de conexión VPN en Intune, consulte [Crear perfiles de VPN para conectarse a los servidores VPN en](https://docs.microsoft.com/intune/vpn-settings-configure)de Intune.  

**La VPN a petición de iOS no se activa cuando se tiene acceso a un dominio configurado**

Para probar la configuración automática de VPN, configure los siguientes valores:

Quiero hacer lo siguiente: **Evaluar cada intento de conexión** 

Elija si quiere conectar: **Conectar si es necesario**

Cuando los usuarios obtienen acceso a estos dominios: **de destino** *nombre de dominio*

Si la configuración anterior no se realiza correctamente, agregue el elemento siguiente:

Cuando no se puede tener acceso a esta dirección URL, obliga a conectar la red privada virtual: **BADURL**