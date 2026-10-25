---
title: "ProjectServerManager.CreateNewProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectServerManager. Crée un nouveau projet dans l'instance Project Server/Project Online en utilisant les options d'enregistrement par défaut"
type: docs
weight: 30
url: /fr/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Crée un nouveau projet dans l'instance Project Server\Project Online en utilisant les options d'enregistrement par défaut.

```csharp
public void CreateNewProject(Project project)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| project | Project | Le projet à enregistrer dans l'instance Project Server\Project Online. |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En cas d'erreur de communication ou d'erreur renvoyée par le serveur. |

## Exemples

Dans cet exemple, le projet est chargé à partir d'un fichier .mpp et enregistré dans le compte Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Montre comment utiliser ProjectServerManager pour créer un nouveau projet sur Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Voir aussi

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Crée un nouveau projet dans une instance de Project Server\Project Online en utilisant les options d’enregistrement spécifiées.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| project | Project | Le projet à enregistrer dans l'instance Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Instance de la classe [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En cas d'erreur de communication ou d'erreur renvoyée par le serveur. |

## Exemples

Dans cet exemple, le projet est chargé à partir d'un fichier .mpp et enregistré dans le compte Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

Montre comment utiliser le gestionnaire Project Server pour créer un nouveau projet avec des options d’enregistrement prédéfinies sur Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Voir aussi

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


