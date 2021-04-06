---
title: Instalar Office y OneDrive en Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590320"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instalar Office y OneDrive en Windows Virtual Desktop

1. [Preparar y personalizar una imagen VHD maestra](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Cree una máquina virtual (VM) si aún no se ha creado.

1. [Instalar Office en el modo de activación en equipos compartidos](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). La activación en equipos compartidos permite a varios usuarios obtener acceso a Office.

1. [Instalar OneDrive en modo por máquina](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Normalmente, OneDrive se instala por usuario. Sin embargo, en este caso debería instalarse por máquina.