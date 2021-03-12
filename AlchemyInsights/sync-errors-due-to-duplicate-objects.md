---
title: 902 (Errores de sincronización debidos a objetos duplicados)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708079"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="0ac5e-102">Errores de sincronización debido a objetos duplicados</span><span class="sxs-lookup"><span data-stu-id="0ac5e-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="0ac5e-103">Es posible que reciba uno de los siguientes mensajes de error cuando finalice la sincronización de directorios en Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="0ac5e-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="0ac5e-104">No se puede actualizar este objeto en Microsoft Online Services porque los siguientes atributos asociados a este objeto tienen valores que ya pueden estar asociados con otro objeto en el directorio local.</span><span class="sxs-lookup"><span data-stu-id="0ac5e-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="0ac5e-105">Ya existe un objeto sincronizado con la misma dirección proxy en el directorio Microsoft Online Services servidor.</span><span class="sxs-lookup"><span data-stu-id="0ac5e-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="0ac5e-106">No se puede actualizar este objeto porque los siguientes atributos asociados a este objeto tienen valores que pueden estar asociados a otro objeto en los servicios de directorio local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="0ac5e-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="0ac5e-107">Para identificar y corregir el problema, descargue y ejecute la herramienta de corrección de [errores IdFix DirSync](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="0ac5e-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="0ac5e-108">Para obtener más información, [vea KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="0ac5e-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
