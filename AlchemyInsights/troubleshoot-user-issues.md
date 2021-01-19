---
title: Solucionar problemas de los usuarios
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886907"
---
# <a name="announcements"></a>Anuncios

Siga las instrucciones de pruebas de compatibilidad de Google para comprobar si las aplicaciones se ven afectadas. La guía de Google está disponible en https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support.

Asegúrese de usar la vista web del sistema o el explorador del sistema al iniciar la sesión de los usuarios con cuentas de Google de consumidor. Para más información, consulte [Cómo iniciar sesión en las aplicaciones solo con el explorador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**No puedo crear un usuario en mi directorio de Azure AD**

Para solucionar el problema de no poder crear un usuario en Azure AD, siga estos pasos:

1. Asegúrese de que está autorizado para crear un nuevo usuario estándar. Solo el rol de administrador global o de administrador de usuarios en Azure Active Directory (AD) puede crear un usuario estándar. Si no tiene uno de estos roles, pida a un administrador que le agregue a uno de estos roles o que cree la nueva cuenta de usuario.
2. Asegúrese de que el nombre de usuario está en un dominio comprobado en su Azure AD. Si no tiene nombres de dominio personalizados comprobados en su Azure AD, puede usar su dominio inicial de Azure AD, que termina con *.onmicrosoft.com.
3. Asegúrese de que el nombre de usuario está en un dominio que no está federado con Azure AD desde su AD local. Los usuarios no se pueden agregar a la nube con nombres de dominio federados desde la implementación local.
4. Asegúrese de que ningún otro usuario o contacto ya tenga el nombre de usuario que desea asignar al nuevo usuario. Los nombres de usuario deben ser únicos en Azure AD.
5. Consulte [Roles y administradores de Azure AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) para su Azure AD.
6. Consulte los [nombres de dominio](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) para su Azure AD.
7. Revise los [Registros de auditoría](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) para ver información más detallada sobre un usuario creado o eliminado recientemente, como quién realizó la acción y cuándo.
8. Para más información sobre cómo agregar nuevos usuarios, consulte [Usar Azure Portal para crear un usuario en Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Para más información sobre los permisos de rol de administrador en Azure AD, consulte [Roles administrativos de Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Para más información sobre cómo crear un usuario con Azure AD PowerShell, vea [Azure AD PowerShell para crear un nuevo usuario](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problema con el registro de autoservicio**

Para solucionar problemas relacionados con el registro de autoservicio, realice los pasos siguientes:

1. Para usar el registro de autoservicio con sus aplicaciones, primero habilite el inicio de sesión de autoservicio para su espacio empresarial. 
2. Para habilitar una aplicación para que admita el registro de autoservicio, agréguela al flujo de usuario. La próxima vez que vaya a la página de inicio de sesión de esa aplicación, verá una opción **_¿No tiene cuenta? Cree una._* _. Esto inicia el proceso de registro de autoservicio.
3. Para obtener información sobre cómo usar el registro de autoservicio para rellenar una organización en Azure AD, consulte [Registro de autoservicio en Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Una vez que asocie el flujo de usuario con una o más aplicaciones, los usuarios que la visiten podrán registrarse y obtener una cuenta de invitado con las opciones configuradas en el flujo de usuario. Para más información sobre cómo suscribirse y obtener una cuenta de invitado, los usuarios pueden ver [Registro de autoservicio para usuarios invitados](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problema al invitar a usuarios externos**

Para solucionar problemas relacionados con la invitación a un usuario externo, realice el siguiente paso:

Asegúrese de enviar la invitación de un usuario a la dirección de correo electrónico que coincida con el nombre con el que el usuario inicia sesión. Si envía la invitación a la dirección de correo electrónico del proxy de un usuario, el usuario no podrá canjearla. Para más información, consulte [Documentación de B2B de Azure AD](https://docs.microsoft.com/azure/active-directory/external-identities/).

**No puedo asignar licencias a un usuario**

Para solucionar los problemas relacionados con la asignación de licencias a un usuario, siga estos pasos:

1. Para administrar licencias de usuario, asegúrese de usar una cuenta con uno de los roles de administrador necesarios: administrador global, administrador de licencias o administrador de usuarios. Puede comprobar el rol del usuario en la pestaña **Rol de directorio** en la hoja de usuario.
2. Si usa Azure Portal y se producen errores al realizar la asignación de licencia, haga clic en la notificación de la esquina superior derecha. Se abrirá una hoja con detalles sobre el problema. En la mayoría de los casos, esto es suficiente para comprender y resolver el problema.
3. Antes de que se pueda asignar una licencia a un usuario, asegúrese de que la propiedad **Ubicación de uso** está establecida para el usuario. Compruebe que el usuario tenga establecida esa propiedad. Para ello, consulte la pestaña **Perfil** en la hoja de usuario.
4. Asegúrese de que hay suficientes licencias disponibles para el producto que intenta asignar. Puede ver el número de licencias disponibles en Azure Portal, en [Azure Active Directory -> Licencias -> Todos los productos](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Es posible que el usuario ya tenga otra licencia cuyos servicios entren en conflicto con los de la nueva licencia que intenta asignar. Por ejemplo, si el usuario tiene habilitado el servicio de Exchange Online (plan 1), no podrá asignar una licencia con Exchange Online (plan 2). Deshabilite uno de los servicios para permitir la nueva asignación de licencia. Si está usando los cmdlets de Azure Portal o PowerShell, la página de **detalles del problema** enumera los servicios específicos que están provocando el conflicto.
6. Si está intentando quitar una licencia que tiene errores, es posible que el usuario tenga otras licencias con servicios que dependen de los servicios que intenta quitar. Si usa los cmdlets de Azure Portal o PowerShell, el mensaje de error mostrará los servicios específicos que tienen dependencias.
7. Si quiere entender por qué se agregó o quitó una licencia a un usuario (por ejemplo, qué otra persona de la organización puede haber realizado cambios), compruebe los registros de auditoría. Establezca el filtro en **actividades de licencias** para mostrar todas las modificaciones, incluido el "autor" que las realizó.
8. Si usa Exchange Online, es posible que algunos usuarios de su espacio empresarial no estén configurados correctamente con el mismo valor de dirección del proxy. En estos casos, es posible que vea mensajes de error genéricos cuando se produce un error en una operación de licencia. [Este artículo](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contiene más información sobre este problema, incluida información sobre [cómo conectarse a Exchange Online con PowerShell remoto](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Para identificar qué usuarios de su espacio empresarial contienen la misma dirección de proxy, ejecute este cmdlet de Exchange Online:

Ejecutar

Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses





