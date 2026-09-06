---
title: "ProjectServerCredentials.ProjectServerCredentials"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "ProjectServerCredentials constructeur. Initialise une nouvelle instance de la classe ProjectServerCredentials en utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le site PWA Project Web Access de SharePoint"
type: docs
weight: 10
url: /fr/net/aspose.tasks/projectservercredentials/projectservercredentials/
---
## ProjectServerCredentials(string, string) {#constructor_1}

Initialise une nouvelle instance de la classe [`ProjectServerCredentials`](../) en utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le PWA (Project Web Access) de SharePoint.

```csharp
public ProjectServerCredentials(string siteUrl, string authToken)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| siteUrl | Chaîne | L'URL de l'API PWA (Project Web Access) de Project Online. |
| authToken | Chaîne | Le jeton d'autorisation (SPOIDCRL) pour le site PWA (Project Web Access) de SharePoint. |

## Remarques

Utilisez ce constructeur pour vous connecter à ProjectOnline lorsque vous disposez déjà d'un AuthToken pour votre site SharePoint Online.

## Exemples

Montre comment utiliser les informations d'identification de Project Server avec SharePointOnlineCredentials pour créer un projet dans Microsoft Project Online.

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

### Voir aussi

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, string, string) {#constructor_2}

Initialise une nouvelle instance de la classe [`ProjectServerCredentials`](../) en utilisant l'URL du site SharePoint, le nom d'utilisateur et le mot de passe.

```csharp
public ProjectServerCredentials(string siteUrl, string userName, string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| siteUrl | Chaîne | L'URL de l'API PWA (Project Web Access) de Project Online. |
| userName | Chaîne | Le nom d'utilisateur pour le site SharePoint. |
| password | Chaîne | Le mot de passe pour le site SharePoint. |

## Remarques

Utilisez ce constructeur pour vous connecter à ProjectOnline. Veuillez noter que l'authentification héritée doit être activée dans votre portail Azure et le centre d'administration Office 365.

## Exemples

Montre comment utiliser les identifiants du serveur de projet pour récupérer la liste des projets depuis Microsoft Project Online.

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

### Voir aussi

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)

---

## ProjectServerCredentials(string, NetworkCredential) {#constructor}

Initialise une nouvelle instance de la classe [`ProjectServerCredentials`](../) en utilisant l'URL du point de terminaison Project Web Access et les informations d'identification réseau.

```csharp
public ProjectServerCredentials(string siteUrl, NetworkCredential credentials)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| siteUrl | Chaîne | L'URL du point de terminaison Project Web Access. |
| identifiants | NetworkCredential | Les informations d'identification utilisées pour se connecter au point de terminaison Project Web Access. |

## Remarques

Utilisez ce constructeur pour vous connecter à une instance locale de Project Server via PWA.

## Exemples

Dans cet exemple, l'instance de la classe [`ProjectServerManager`](../../projectservermanager/) est utilisée pour lire une liste de projets depuis l'instance de Project Server située à http://project_server_instance.local

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

Montre comment utiliser les informations d'identification de Project Server avec des informations d'identification réseau pour lire un projet depuis une instance locale de Project Server.

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

### Voir aussi

* class [ProjectServerCredentials](../)
* namespace [Aspose.Tasks](../../projectservercredentials/)
* assembly [Aspose.Tasks](../../../)


