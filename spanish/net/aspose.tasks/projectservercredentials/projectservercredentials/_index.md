---
title: ProjectServerCredentials.ProjectServerCredentials
second_title: Referencia de Aspose.Tasks para la API de .NET
description: ProjectServerCredentials constructor. Inicializa una nueva instancia delProjectServerCredentials class usando la URL del sitio de SharePoint y el token de autorización SPOIDCRL válido para el sitio PWA Project Web Access de SharePoint.
type: docs
weight: 10
url: /es/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Inicializa una nueva instancia del[`ProjectServerCredentials`](../) class usando la URL del sitio de SharePoint y el token de autorización SPOIDCRL válido para el sitio PWA (Project Web Access) de SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| siteUrl | String | La URL de la API de PWA (Project Web Access) de Project Online. |
| authToken | String | El token de autorización (SPOIDCRL) para el sitio PWA (Project Web Access) de SharePoint. |

### Observaciones

Use este constructor para conectarse a ProjectOnline cuando ya tenga AuthToken para su sitio de SharePoint Online.

### Ver también

* class [ProjectServerCredentials](../)
* espacio de nombres [Aspose.Tasks](../../projectservercredentials/)
* asamblea [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Inicializa una nueva instancia del[`ProjectServerCredentials`](../) clase usando la URL del sitio de SharePoint, nombre de usuario y contraseña.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| siteUrl | String | La URL de la API de PWA (Project Web Access) de Project Online. |
| userName | String | El nombre de usuario del sitio de SharePoint. |
| password | String | La contraseña para el sitio de SharePoint. |

### Observaciones

Utilice este constructor para conectarse a ProjectOnline. Tenga en cuenta que la autenticación heredada debe estar habilitada en su Azure Portal y en el centro de administración de Office 365.

### Ver también

* class [ProjectServerCredentials](../)
* espacio de nombres [Aspose.Tasks](../../projectservercredentials/)
* asamblea [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Inicializa una nueva instancia del[`ProjectServerCredentials`](../) class usando la URL del extremo de Project Web Access y las credenciales de red.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| siteUrl | String | La URL del punto final de acceso web del proyecto. |
| credentials | NetworkCredential | Las credenciales utilizadas para iniciar sesión en el extremo de Project Web Access. |

### Observaciones

Use este constructor para conectarse a la instancia local de Project Server a través de PWA.

### Ejemplos

En este ejemplo, la instancia de[`ProjectServerManager`](../../projectservermanager/)La clase se usa para leer una lista de proyectos de la instancia de Project Server ubicada en http://project_server_instance.local

```csharp
string site = "http://proyecto_servidor_instancia.local/sitios/pwa";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

### Ver también

* class [ProjectServerCredentials](../)
* espacio de nombres [Aspose.Tasks](../../projectservercredentials/)
* asamblea [Aspose.Tasks](../../../)


