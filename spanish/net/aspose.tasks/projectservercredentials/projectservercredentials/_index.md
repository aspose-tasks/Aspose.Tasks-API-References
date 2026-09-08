---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor ProjectServerCredentials. Inicializa una nueva instancia de la clase ProjectServerCredentials usando la URL del sitio de SharePoint y un token de autorización SPOIDCRL válido para el sitio PWA Project Web Access de SharePoint"
type: docs
weight: 10
url: /es/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Inicializa una nueva instancia de la clase [`ProjectServerCredentials`](../) usando la URL del sitio de SharePoint y un token de autorización SPOIDCRL válido para el PWA (Project Web Access) de SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| siteUrl | Cadena | La URL de la API PWA (Project Web Access) de Project Online. |
| authToken | Cadena | El token de autorización (SPOIDCRL) para el sitio PWA (Project Web Access) de SharePoint. |

## Observaciones

Utilice este constructor para conectarse a ProjectOnline cuando ya tenga AuthToken para su sitio SharePoint Online.

## Ejemplos

Muestra cómo usar credenciales de Project Server con SharePointOnlineCredentials para crear un proyecto en Microsoft Project Online.

```csharp
try
{
    const string Username = "admin@contoso.onmicrosoft.com";
    const string SecuredPassword = "MyPassword";
    var url = new Uri("https://contoso.sharepoint.com/sites/pwa");
    var project = new Project(DataDir + "Project1.mpp");
    var password = new SecureString();
    foreach (var c in SecuredPassword)
    {
        password.AppendChar(c);
    }

    var onlineCredentials = new SharePointOnlineCredentials(Username, password);
    var projectServerCredentials = new ProjectServerCredentials(url.ToString(), onlineCredentials.GetAuthenticationCookie(url, true));

    Console.WriteLine("Project Server Auth Token: " + projectServerCredentials.AuthToken);
    Console.WriteLine("Project Server Site Url: " + projectServerCredentials.SiteUrl);
    Console.WriteLine("Project Server User Name: " + projectServerCredentials.UserName);

    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Inicializa una nueva instancia de la clase [`ProjectServerCredentials`](../) usando la URL del sitio SharePoint, nombre de usuario y contraseña.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| siteUrl | Cadena | La URL de la API PWA (Project Web Access) de Project Online. |
| userName | Cadena | El nombre de usuario para el sitio SharePoint. |
| password | Cadena | La contraseña para el sitio SharePoint. |

## Observaciones

Utilice este constructor para conectarse a ProjectOnline. Tenga en cuenta que la autenticación heredada debe estar habilitada en su portal de Azure y en el centro de administración de Office 365.

## Ejemplos

Muestra cómo usar credenciales de Project Server para obtener la lista de proyectos de Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Inicializa una nueva instancia de la clase [`ProjectServerCredentials`](../) usando la URL del punto final de Project Web Access y credenciales de red.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| siteUrl | Cadena | La URL del punto final de Project Web Access. |
| credenciales | NetworkCredential | Las credenciales usadas para iniciar sesión en el punto final de Project Web Access. |

## Observaciones

Utilice este constructor para conectarse a una instancia local de Project Server a través de PWA.

## Ejemplos

En este ejemplo, la instancia de la clase [`ProjectServerManager`](../../projectservermanager/) se usa para leer una lista de proyectos de la instancia de Project Server ubicada en http://project_server_instance.local

```csharp
string site = "http://project_server_instance.local/sites/pwa";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);

var list = manager.GetProjectList();
foreach (var projectInfo in list)
{
    Console.WriteLine("{0} - {1} - {2}", projectInfo.Id, projectInfo.CreatedDate, projectInfo.Name);
}
```

Muestra cómo usar credenciales de Project Server con credenciales de red para leer un proyecto de una instancia local de Project Server.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


