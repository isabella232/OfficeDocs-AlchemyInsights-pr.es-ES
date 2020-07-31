---
title: Perfiles de Wi-Fi de Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509076"
---
# <a name="intune-wi-fi-profiles"></a>Perfiles de Wi-Fi de Intune

La implementación correcta de conectividad Wi-Fi para los clientes MDM depende de un perfil correctamente implementado que refleja los requisitos de la infraestructura de Wi-Fi corporativa. Para revisar la configuración adecuada para las plataformas de cliente que está investigando, consulte: 

[Agregar la configuración de Wi-Fi para dispositivos que ejecutan Android en Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Agregar la configuración de Wi-Fi para dispositivos Android Enterprise dedicados y totalmente administrados en Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Agregar la configuración de Wi-Fi para dispositivos iOS e iPadOS en Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Agregar la configuración de Wi-Fi para dispositivos con Windows 10 y versiones posteriores en Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importar la configuración de Wi-Fi para dispositivos con Windows en Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Problemas comunes**

**Estoy implementando un perfil de Wi-Fi que depende de un certificado implementado especificado en el perfil de Wi-Fi. Sin embargo, los perfiles de configuración muestran un estado de error.**

Compruebe la recepción del certificado en el dispositivo.

1. En Intune, vaya a **Todos los dispositivos** y seleccione el dispositivo > **Configuración del dispositivo**.

2. Compruebe que todos los perfiles previstos estén enumerados y en un estado correcto.

3. Para un perfil Android, si tiene certificados intermedios en la cadena de certificados, asegúrese de que se implementen en dispositivos Android.

    Para comprobar el estado del certificado, vaya a **Configuración del dispositivo** > **Perfiles** > **Entidad de certificación intermedio de Android** > **Propiedades** > **Certificado de confianza**.

Si aún observa errores, revise los procedimientos y las secciones de solución de problemas. Para obtener más información, consulte [Información general sobre la solución de problemas de perfiles de certificado SCEP con Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Desplegó un perfil de Wi-Fi en un dispositivo. Intune muestra que se completó correctamente, pero el dispositivo no se conecta al Wi-Fi.**

Un estado correcto significa que Intune ha implementado correctamente el perfil como configurado. Sin embargo, estas configuraciones podrían no coincidir con los requisitos de red y/o autenticación. Para más información sobre el intento de conexión, revise los registros en el servicio de autenticación e infraestructura (en el controlador del punto de acceso Wi-Fi y el servidor NPS/RADIUS). Es posible que tenga que colaborar con el equipo de infraestructura de red o el proveedor de Wi-Fi de terceros para recopilar y revisar registros.