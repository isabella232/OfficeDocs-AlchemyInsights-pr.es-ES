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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="0dcdf-102">Conector local de Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="0dcdf-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="0dcdf-103">Para obtener información detallada sobre cómo configurar el conector entre Intune y Exchange hospedado de forma local, vea la siguiente documentación:</span><span class="sxs-lookup"><span data-stu-id="0dcdf-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="0dcdf-104">Configurar el conector de Exchange local de Intune en Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="0dcdf-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="0dcdf-105">**Preguntas más frecuentes:**</span><span class="sxs-lookup"><span data-stu-id="0dcdf-105">**FAQ:**</span></span>

<span data-ttu-id="0dcdf-106">P: aparece un error como "no se admite la versión del conector de Exchange" al intentar configurar el conector de Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="0dcdf-107">¿Qué puede ser la causa?</span><span class="sxs-lookup"><span data-stu-id="0dcdf-107">What could be the cause?</span></span>

<span data-ttu-id="0dcdf-108">A: la cuenta que está usando tiene una licencia adecuada: debe tener una licencia activa de Intune</span><span class="sxs-lookup"><span data-stu-id="0dcdf-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="0dcdf-109">P: ¿es posible tener varios conectores de Exchange?</span><span class="sxs-lookup"><span data-stu-id="0dcdf-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="0dcdf-110">A: solo puede configurar un conector de Exchange por cada organización de Exchange para cada inquilino de Intune.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="0dcdf-111">El conector solo se puede instalar en un servidor de una organización de Exchange de varios servidores.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="0dcdf-112">Tampoco puede tener conectores configurados para Exchange local y Exchange Online configurados en el mismo inquilino.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="0dcdf-113">P: ¿puede el conector usar una matriz CAS como conexión con Exchange?</span><span class="sxs-lookup"><span data-stu-id="0dcdf-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="0dcdf-114">A: no se admite la especificación de una matriz CAS en la configuración del conector.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="0dcdf-115">Solo debe especificarse un único servidor y codificarse en el archivo de configuración del conector, que se puede encontrar en</span><span class="sxs-lookup"><span data-stu-id="0dcdf-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="0dcdf-116">Programa data\microsoft\microsoft Intune en el conector de Exchange local \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="0dcdf-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="0dcdf-117">Busque la entrada siguiente ```<ExchangeWebServiceURL />``` y reemplace la dirección URL con el servidor de Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="0dcdf-118">**Siguiente**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="0dcdf-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="0dcdf-119">Consulte la siguiente documentación para obtener más información sobre solución de problemas: [solución de problemas del conector de Exchange local de Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune) .</span><span class="sxs-lookup"><span data-stu-id="0dcdf-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="0dcdf-120">**Habilitación del registro detallado para el conector de Exchange**</span><span class="sxs-lookup"><span data-stu-id="0dcdf-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="0dcdf-121">Abra el archivo de configuración de seguimiento de conectores de Exchange para su edición.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="0dcdf-122">El archivo se encuentra en:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="0dcdf-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="0dcdf-123">**Siguiente**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="0dcdf-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="0dcdf-124">Busque TraceSourceLine con la siguiente clave: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="0dcdf-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="0dcdf-125">Cambie el valor del nodo SourceLevel de la información ActivityTracing (opción predeterminada) a ActivityTracing detallado.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="0dcdf-126">**Ejemplo:**</span><span class="sxs-lookup"><span data-stu-id="0dcdf-126">**Example:**</span></span>
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
4. <span data-ttu-id="0dcdf-127">Reiniciar el servicio de Exchange de Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0dcdf-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="0dcdf-128">Sincronización completa en el portal de Intune hasta que finalice y, a continuación, vuelva a cambiar el XML a "Information ActivityTracing" y reinicie el servicio de Exchange de Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="0dcdf-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="0dcdf-129">La ubicación de los registros es: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="0dcdf-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>