---
title: Conceptos de autenticación avanzada aplicables a Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571893"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="b198e-102">Conceptos de autenticación avanzada aplicables a Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b198e-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="b198e-103">A continuación se muestran los conceptos de autenticación avanzada aplicables a Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="b198e-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="b198e-104">**Autenticación proactiva**</span><span class="sxs-lookup"><span data-stu-id="b198e-104">**Proactive Authentication**</span></span>

<span data-ttu-id="b198e-105">Al habilitar la directiva [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge intentará autenticar de forma proactiva los usuarios que han iniciado sesión a través de los servicios de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b198e-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="b198e-106">A intervalos regulares, usará un servicio en línea para comprobar si hay un manifiesto actualizado que contenga la configuración que rige la autenticación proactiva.</span><span class="sxs-lookup"><span data-stu-id="b198e-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="b198e-107">Ventajas: la autenticación proactiva permite la autenticación a los servicios clave, como la página de la nueva pestaña de Office.</span><span class="sxs-lookup"><span data-stu-id="b198e-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="b198e-108">Además, si se usa Bing como motor de búsqueda, la autenticación proactiva mejora el rendimiento de la barra de direcciones y ayuda a generar resultados de búsqueda personalizados para las necesidades de su empresa.</span><span class="sxs-lookup"><span data-stu-id="b198e-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="b198e-109">**Windows Hello CredUI para la autenticación NTLM**</span><span class="sxs-lookup"><span data-stu-id="b198e-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="b198e-110">Si el inicio de sesión único (SSO) no está disponible cuando un sitio web intenta iniciar sesión en el usuario mediante el mecanismo NTLM o Negotiate, esta característica permitirá al usuario compartir las credenciales del sistema operativo con el sitio web y cumplir el desafío de autenticación mediante la interfaz de usuario CRED de Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="b198e-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="b198e-111">Este flujo de inicio de sesión solo aparecerá en Windows 10 y solo para los usuarios que no reciban SSO durante un desafío de NTLM o de negociación.</span><span class="sxs-lookup"><span data-stu-id="b198e-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="b198e-112">**Usar contraseñas guardadas para iniciar sesión automáticamente**</span><span class="sxs-lookup"><span data-stu-id="b198e-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="b198e-113">Los usuarios que guardan contraseñas en Microsoft Edge pueden habilitar el inicio de sesión automático en los sitios web donde tienen credenciales guardadas.</span><span class="sxs-lookup"><span data-stu-id="b198e-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="b198e-114">Los usuarios pueden activar o desactivar esta característica en edge://settings/passwords, y puede configurarla en las directivas del [Administrador de contraseñas](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="b198e-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
