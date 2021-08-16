---
title: Intune Exchange local Connector
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013981"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange local Connector

Para obtener más información sobre cómo configurar el conector entre Intune y Exchange que se hospeda localmente, consulte la siguiente documentación:

[Configurar el conector de configuración local de Intune Exchange en Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Preguntas más frecuentes:**

P: Veo un error como "No se admite la versión de Exchange Connector" al intentar configurar el Exchange conector. ¿Cuál podría ser la causa?

A: La cuenta que está usando tiene una licencia adecuada: debe tener una licencia activa de Intune

P: ¿Es posible tener varios Exchange conectores?

A: Solo puede configurar un conector de Exchange por inquilino de Intune por cada Exchange organización. El conector solo se puede instalar en un servidor de una organización de intercambio de varios servidores.

Tampoco puede tener conectores configurados para Exchange local y Exchange Online configurados en el mismo espacio empresarial.

P: ¿Puede el conector usar una matriz CAS como conexión a Exchange?

A: Especificar una matriz CAS no es una configuración compatible en la configuración del conector. Solo se debe especificar un único servidor y debe estar codificado de forma rígida en el archivo de configuración del conector que se puede encontrar en

datos del programa\microsoft\microsoft Intune local Exchange conector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Busque la siguiente entrada ```<ExchangeWebServiceURL />``` y reemplace la dirección URL por el servidor exchange.

**Ejemplo:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Consulte la siguiente documentación para obtener más información sobre la solución de problemas: Solucionar problemas del conector [Exchange Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Habilitar el registro detallado para el Exchange de datos**

1. Abra el archivo de configuración Exchange de seguimiento de Connector para editarlo.  
El archivo se encuentra en : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Ejemplo:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Busque TraceSourceLine con la siguiente clave: OnPremisesExchangeConnectorService  
  
3. Cambiar el valor del nodo SourceLevel de Information ActivityTracing (valor predeterminado) a Verbose ActivityTracing  

**Ejemplo:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Reiniciar el servicio Microsoft Intune Exchange de Microsoft Intune Exchange  
5. Sincronización completa en Intune Portal hasta que finalice y, a continuación, vuelva a cambiar el XML a "Information ActivityTracing" y reinicie el Microsoft Intune Exchange web.  
6. La ubicación de los registros es: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`