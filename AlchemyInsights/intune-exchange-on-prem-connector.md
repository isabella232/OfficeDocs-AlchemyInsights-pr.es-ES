---
title: Conector local de Intune Exchange
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
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791598"
---
# <a name="intune-exchange-on-premise-connector"></a>Conector local de Intune Exchange

Para obtener información detallada sobre cómo configurar el conector entre Intune y Exchange hospedado de forma local, vea la siguiente documentación:

[Configurar el conector de Exchange local de Intune en Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Preguntas más frecuentes:**

P: aparece un error como "no se admite la versión del conector de Exchange" al intentar configurar el conector de Exchange. ¿Qué puede ser la causa?

A: la cuenta que está usando tiene una licencia adecuada: debe tener una licencia activa de Intune

P: ¿es posible tener varios conectores de Exchange?

A: solo puede configurar un conector de Exchange por cada organización de Exchange para cada inquilino de Intune. El conector solo se puede instalar en un servidor de una organización de Exchange de varios servidores.

Tampoco puede tener conectores configurados para Exchange local y Exchange Online configurados en el mismo inquilino.

P: ¿puede el conector usar una matriz CAS como conexión con Exchange?

A: no se admite la especificación de una matriz CAS en la configuración del conector. Solo debe especificarse un único servidor y codificarse en el archivo de configuración del conector, que se puede encontrar en

Programa data\microsoft\microsoft Intune en el conector de Exchange local \ OnpremiseExchangeConnectorServiceConfiguration.xml

Busque la entrada siguiente ```<ExchangeWebServiceURL />``` y reemplace la dirección URL con el servidor de Exchange.

**Siguiente**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Consulte la siguiente documentación para obtener más información sobre solución de problemas: [solución de problemas del conector de Exchange local de Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune) .

**Habilitación del registro detallado para el conector de Exchange**

1. Abra el archivo de configuración de seguimiento de conectores de Exchange para su edición.  
El archivo se encuentra en:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Siguiente**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Busque TraceSourceLine con la siguiente clave: OnPremisesExchangeConnectorService  
  
3. Cambie el valor del nodo SourceLevel de la información ActivityTracing (opción predeterminada) a ActivityTracing detallado.  

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
4. Reiniciar el servicio de Exchange de Microsoft Intune  
5. Sincronización completa en el portal de Intune hasta que finalice y, a continuación, vuelva a cambiar el XML a "Information ActivityTracing" y reinicie el servicio de Exchange de Microsoft Intune.  
6. La ubicación de los registros es: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`