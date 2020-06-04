---
title: Creación de directivas de etiquetas de AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542195"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="6ff47-102">Creación de directivas de etiquetas de AIP</span><span class="sxs-lookup"><span data-stu-id="6ff47-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="6ff47-103">Las etiquetas de Azure Information Protection (AIP) se pueden usar con el rango completo de datos que una organización crea y almacena, desde la clasificación más baja de datos personales, hasta la clasificación más alta de los datos extremadamente confidenciales.</span><span class="sxs-lookup"><span data-stu-id="6ff47-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="6ff47-104">Las directivas de Azure Information Protection se aplican al cliente clásico de Azure Information Protection (AIP) y no al [cliente de etiquetado Unificado de AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="6ff47-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="6ff47-105">Puede configurar varios elementos en una directiva de AIP, incluidas opciones como:</span><span class="sxs-lookup"><span data-stu-id="6ff47-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="6ff47-106">Opción para la que Label permitirá a los administradores o los documentos y mensajes de correo electrónico de clasificación y protección (opcional)</span><span class="sxs-lookup"><span data-stu-id="6ff47-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="6ff47-107">Opción para aplicar la clasificación cuando los usuarios guardan documentos y envían correo electrónico</span><span class="sxs-lookup"><span data-stu-id="6ff47-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="6ff47-108">Opción para etiquetar automáticamente un mensaje de correo electrónico basándose en sus datos adjuntos.</span><span class="sxs-lookup"><span data-stu-id="6ff47-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="6ff47-109">Opción para controlar si la barra de protección de la información se muestra en las aplicaciones de Office</span><span class="sxs-lookup"><span data-stu-id="6ff47-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="6ff47-110">Para obtener más opciones e información sobre las directivas de Azure Information Protection, consulte: [información general sobre la Directiva de Azure Information Protection](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="6ff47-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="6ff47-111">Para obtener más recursos útiles sobre las directivas de AIP, consulte:</span><span class="sxs-lookup"><span data-stu-id="6ff47-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="6ff47-112">Tutorial: configurar las opciones de directiva de Azure Information Protection y crear una nueva etiqueta</span><span class="sxs-lookup"><span data-stu-id="6ff47-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="6ff47-113">Configuración de la Directiva de Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6ff47-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="6ff47-114">Crear y configurar etiquetas de confidencialidad y sus directivas</span><span class="sxs-lookup"><span data-stu-id="6ff47-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="6ff47-115">Guías de procedimientos para escenarios comunes que usan Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6ff47-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="6ff47-116">Revisar la documentación de Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6ff47-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="6ff47-117">Requisitos para Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6ff47-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="6ff47-118">Tutorial de inicio rápido para Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6ff47-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="6ff47-119">Descargar el cliente de Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6ff47-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)