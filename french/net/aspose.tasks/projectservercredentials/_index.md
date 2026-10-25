---
title: "Classe ProjectServerCredentials"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ProjectServerCredentials. Identifiants utilisés pour se connecter à Project Online ou à une instance sur site de Project Server"
type: docs
weight: 1490
url: /fr/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Identifiants utilisés pour se connecter à Project Online ou à une instance sur site de Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Initialise une nouvelle instance de la classe `ProjectServerCredentials` en utilisant l'URL du point de terminaison Project Web Access et les identifiants réseau. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Initialise une nouvelle instance de la classe `ProjectServerCredentials` en utilisant l'URL du site SharePoint et un jeton d'autorisation SPOIDCRL valide pour le site PWA (Project Web Access) de SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Initialise une nouvelle instance de la classe `ProjectServerCredentials` en utilisant l'URL du site SharePoint, le nom d'utilisateur et le mot de passe. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Obtient le jeton d'autorisation pour l'instance SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Obtient l'URL du PWA sur le site SharePoint ou l'URL du Project Server sur site. Par exemple, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Obtient le nom d'utilisateur pour le site SharePoint. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Renvoie une représentation sous forme de chaîne de cette instance. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


