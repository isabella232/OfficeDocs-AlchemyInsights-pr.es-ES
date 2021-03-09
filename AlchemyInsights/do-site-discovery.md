---
title: Realizar detección de sitio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529310"
---
# <a name="do-site-discovery"></a><span data-ttu-id="6a838-102">Realizar detección de sitio</span><span class="sxs-lookup"><span data-stu-id="6a838-102">Do site discovery</span></span>

<span data-ttu-id="6a838-103">Si su organización todavía utiliza aplicaciones web heredadas y planea usar el modo Internet Explorer (lo que hacen la mayoría de los clientes), debería realizar una detección adicional del sitio.</span><span class="sxs-lookup"><span data-stu-id="6a838-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="6a838-104">**Ya ha implementado una versión anterior de Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="6a838-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="6a838-105">Si ya ha configurado su lista de sitios de empresa para que funcione con la versión heredada de Microsoft Edge, la detección de sitio ya casi ha finalizado.</span><span class="sxs-lookup"><span data-stu-id="6a838-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="6a838-106">Puede que necesite agregar sitios neutros.</span><span class="sxs-lookup"><span data-stu-id="6a838-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="6a838-107">Los sitios neutros son normalmente sitios que proporcionan inicio de sesión único (SSO).</span><span class="sxs-lookup"><span data-stu-id="6a838-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="6a838-108">Si va a un sitio neutro desde Microsoft Edge, es conveniente que se quede en Microsoft Edge para autenticarse.</span><span class="sxs-lookup"><span data-stu-id="6a838-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="6a838-109">Si va a un sitio neutro desde el modo Internet Explorer, es conveniente que se quede en el modo Internet Explorer para autenticarse.</span><span class="sxs-lookup"><span data-stu-id="6a838-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="6a838-110">Identifique cualquier sitio SSO u otros sitios neutros que use y agréguelos a su lista de sitios de empresa.</span><span class="sxs-lookup"><span data-stu-id="6a838-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="6a838-111">**Internet Explorer es su explorador predeterminado**</span><span class="sxs-lookup"><span data-stu-id="6a838-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="6a838-112">Si actualmente solo usa Internet Explorer, es posible que no sepa qué sitios se han actualizado a los estándares web modernos y cuáles requieren todavía Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6a838-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="6a838-113">Es recomendable encontrar y agregar estos sitios a la lista de sitios de empresa para poder utilizar el modo Internet Explorer solo para esos sitios.</span><span class="sxs-lookup"><span data-stu-id="6a838-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="6a838-114">[Detección de sitio de empresa](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) detecta los sitios que pueden necesitar el modo Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6a838-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="6a838-115">Puede recopilar datos de equipos que ejecutan Windows Internet Explorer 8 a través de Internet Explorer 11 en Windows 10, Windows 8.1 o Windows 7.</span><span class="sxs-lookup"><span data-stu-id="6a838-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="6a838-116">**Analizar los datos**</span><span class="sxs-lookup"><span data-stu-id="6a838-116">**Analyze the data**</span></span>

<span data-ttu-id="6a838-117">Una vez que haya recopilado los datos del sitio, recomendamos seguir un proceso de cuatro pasos para analizar los datos:</span><span class="sxs-lookup"><span data-stu-id="6a838-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="6a838-118">Ordenar los datos por dominio y, a continuación, por URL.</span><span class="sxs-lookup"><span data-stu-id="6a838-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="6a838-119">Definir los límites de una aplicación para configurarla para el modo Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6a838-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="6a838-120">Es recomendable incluir todos los sitios y controles web que definan la aplicación, pero sin incluir controles y sitios extra.</span><span class="sxs-lookup"><span data-stu-id="6a838-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="6a838-121">Algunos sitios pueden ser tan sencillos como *https://contoso.com/app1*, mientras que otros pueden requerir que definas varios sitios y páginas.</span><span class="sxs-lookup"><span data-stu-id="6a838-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="6a838-122">Prueba la aplicación para comprobar que no funciona de forma nativa.</span><span class="sxs-lookup"><span data-stu-id="6a838-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="6a838-123">Muchos sitios ofrecerán contenido moderno cuando detecten un explorador moderno y solo ofrecerán contenido heredado cuando detecten Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6a838-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="6a838-124">Agrega la aplicación a la lista de sitios de empresa si la prueba no se realiza correctamente.</span><span class="sxs-lookup"><span data-stu-id="6a838-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="6a838-125">Como práctica recomendada, agrupa todos los sitios que componen una aplicación.</span><span class="sxs-lookup"><span data-stu-id="6a838-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="6a838-126">De esta manera, al actualizar una aplicación, es más sencillo eliminar todo el sitio del modo Internet Explorer y empezar a usar un explorador moderno para esa aplicación.</span><span class="sxs-lookup"><span data-stu-id="6a838-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="6a838-127">Una vez que haya finalizado la detección de sitio y haya analizado los datos, podrá empezar a ocuparse de su estrategia de canal.</span><span class="sxs-lookup"><span data-stu-id="6a838-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

