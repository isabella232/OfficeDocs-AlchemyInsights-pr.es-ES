---
title: Agregar usuarios externos a un grupo de distribución
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934850"
---
# <a name="add-external-users-to-a-distribution-group"></a>Agregar usuarios externos a un grupo de distribución

Agregar un contacto externo a un grupo de distribución (DG) es un proceso de dos pasos:
  
1. Crear un contacto de correo para el usuario externo:
    
    1. En el Centro de administración, vaya a la **página Contactos**  >  [de](https://admin.microsoft.com/adminportal/home#/Contact) usuarios. 
    
    2. Seleccione **Agregar un contacto**.
    
    3. Escriba la información de su contacto y seleccione **Agregar**.
    
2. Agregue el contacto de correo a su DG:
    
    1. En el Centro de administración, vaya a la **página Grupos.**  >  [](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Busque la DG a la que desea agregar el usuario externo y selecciónelo para abrir el cuadro de diálogo de edición.
    
    3. En la **pestaña Miembros,** seleccione **Ver todos y administrar miembros**. 
    
    4. Seleccione **Agregar miembros**.
    
    5. Seleccione el contacto de correo que creó en el paso anterior y, a continuación, **seleccione Guardar**.
    
Si después de seguir estos pasos los usuarios externos no pueden enviar correos electrónicos a la DG o no recibir correos electrónicos de él, podría ser que la DIRECCIÓN GENERAL esté marcada para permitir solo correos electrónicos de usuarios internos. Puede comprobar esta configuración y corregirla siguiendo las instrucciones [aquí](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Nota:** Estas instrucciones no se aplican si el tipo del grupo es "Microsoft 365 grupo" en lugar de "Grupo de distribución". Si ese es el caso, puede agregar el usuario externo directamente al grupo desde Outlook. Encontrará información detallada sobre Microsoft 365 grupos de invitados, así como instrucciones para agregar invitados externos en [este artículo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  