---
title: Configurar el punto de conexión de servicio (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898067"
---
# <a name="configure-service-connection-point-scp"></a>Configurar el punto de conexión de servicio (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Motivo**: no se puede leer el objeto SCP y obtener la información del inquilino de Azure AD
- **Resolución**: consulte la sección [Configurar un punto de conexión de servicio](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Plan de acción**

- Compruebe si el dispositivo ha recibido el GPO para la validación controlada.
- Asegúrese de que el GPO haya creado las claves de registro.
- Asegúrese de tener dos claves creadas con su identificador de directorio y dominio de onmicrosoft.

**Ajustar la configuración del registro del lado cliente para SCP**

Utilice el siguiente ejemplo para crear un objeto de directiva de grupo (GPO) para implementar una configuración de registro que configure una entrada de SCP en el registro de sus dispositivos.

1. Abra una consola de administración de directiva de grupo y cree un nuevo GPO en el dominio.
     - Proporcione un nombre a su GPO recién creado (por ejemplo, ClientSideSCP)

2. Edite el GPO y localice la siguiente ruta: **Configuración del equipo > Preferencias > Configuración de Windows > Registro**.

3. Haga clic derecho en **Registro** y seleccione **Nuevo > Elemento de registro**.

4. En la pestaña **General**, configure los ajustes siguientes:
  
- **Acción**: actualizar
    
- **Subárbol**: HKEY_LOCAL_MACHINE
    
- **Ruta clave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nombre del valor**: TenantId
    
- **Tipo de valor**: REG_SZ
    
- **Datos del valor**: El GUID o Identificador de directorio de la instancia de Azure AD (este valor se puede encontrar en **Azure Portal > Azure Active Directory > Propiedades > Identificador de directorio**)
 
- Haga clic en **Aceptar**.
 
5. Haga clic derecho en **Registro** y seleccione **Nuevo > Elemento de registro**.

6. En la pestaña **General**, configure los ajustes siguientes:
  
- **Acción**: actualizar
    
- **Subárbol**: HKEY_LOCAL_MACHINE
    
- **Ruta clave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nombre del valor**: TenantName
    
- **Tipo de valor**: REG_SZ
    
- **Datos del valor**: el nombre de dominio verificado si utiliza un entorno federado como AD FS. El nombre de dominio verificado o el nombre de dominio onmicrosoft.com (por ejemplo, contoso.onmicrosoft).com si está utilizando un entorno administrado

- Haga clic en **Aceptar**.

7. Cierre el editor del GPO recién creado.

8. Vincule el GPO recién creado a la unidad organizativa deseada que contenga equipos unidos a un dominio que pertenezcan a su conjunto de datos de implementación controlado.

Para obtener más información, consulte [Validación controlada de la Unión a Azure AD híbrido: Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) y [Solución de problemas de dispositivos de Unión a Azure AD híbrido | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









