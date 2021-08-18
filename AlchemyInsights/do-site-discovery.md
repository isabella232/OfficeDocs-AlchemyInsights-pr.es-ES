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
ms.openlocfilehash: 5ae99192c769dd5d5acae1c6e8f9b021e824b465
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322184"
---
# <a name="do-site-discovery"></a>Realizar detección de sitio

Si su organización todavía utiliza aplicaciones web heredadas y planea usar el modo Internet Explorer (lo que hacen la mayoría de los clientes), debería realizar una detección adicional del sitio.

**Ya ha implementado una versión anterior de Microsoft Edge**

Si ya ha configurado su lista de sitios de empresa para que funcione con la versión heredada de Microsoft Edge, la detección de sitio ya casi ha finalizado. Puede que necesite agregar sitios neutros.

Los sitios neutros son normalmente sitios que proporcionan inicio de sesión único (SSO). Si va a un sitio neutro desde Microsoft Edge, es conveniente que se quede en Microsoft Edge para autenticarse. Si va a un sitio neutro desde el modo Internet Explorer, es conveniente que se quede en el modo Internet Explorer para autenticarse.

Identifique cualquier sitio SSO u otros sitios neutros que use y agréguelos a su lista de sitios de empresa.

**Internet Explorer es su explorador predeterminado**

Si actualmente solo usa Internet Explorer, es posible que no sepa qué sitios se han actualizado a los estándares web modernos y cuáles requieren todavía Internet Explorer. Es recomendable encontrar y agregar estos sitios a la lista de sitios de empresa para poder utilizar el modo Internet Explorer solo para esos sitios.

**Nota**: [Detección de sitio de empresa](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) detecta los sitios que pueden necesitar el modo Internet Explorer. Puede recopilar datos de equipos que ejecutan Windows Internet Explorer 8 a través de Internet Explorer 11 en Windows 10, Windows 8.1 o Windows 7.

**Analizar los datos**

Una vez que haya recopilado los datos del sitio, recomendamos seguir un proceso de cuatro pasos para analizar los datos:
1. Ordenar los datos por dominio y, a continuación, por URL.
2. Definir los límites de una aplicación para configurarla para el modo Internet Explorer. Es recomendable incluir todos los sitios y controles web que definan la aplicación, pero sin incluir controles y sitios extra. Algunos sitios pueden ser tan sencillos como *https://contoso.com/app1*, mientras que otros pueden requerir que definas varios sitios y páginas.
3. Pruebe la aplicación para comprobar que no funciona de forma nativa. Muchos sitios ofrecerán contenido moderno cuando detecten un explorador moderno y solo ofrecerán contenido heredado cuando detecten Internet Explorer.
4. Agrega la aplicación a la lista de sitios de empresa si la prueba no se realiza correctamente.

**Nota**: como práctica recomendada, agrupa todos los sitios que componen una aplicación. De esta manera, al actualizar una aplicación, es más sencillo eliminar todo el sitio del modo Internet Explorer y empezar a usar un explorador moderno para esa aplicación.

Una vez que haya finalizado la detección de sitio y haya analizado los datos, podrá empezar a ocuparse de su estrategia de canal.

