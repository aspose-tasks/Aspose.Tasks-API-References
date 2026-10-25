---
title: "Classe ProjectServerManager"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ProjectServerManager. La classe qui fournit les méthodes pour lire et effectuer des opérations sur les projets dans le compte Project Online spécifié ou dans l'instance Project Server sur site spécifiée. Les versions de Project Server 2016 et 2019 sont prises en charge."
type: docs
weight: 1500
url: /fr/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

La classe qui fournit les méthodes pour lire et effectuer des opérations sur les projets dans le compte Project Online spécifié ou dans l'instance sur site de Project Server spécifiée (les versions 2016 et 2019 de Project Server sont prises en charge).

```csharp
public sealed class ProjectServerManager
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Initialise une nouvelle instance de la classe `ProjectServerManager`. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Crée un nouveau projet dans l'instance Project Server\Project Online en utilisant les options d'enregistrement par défaut. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Crée un nouveau projet dans une instance de Project Server\Project Online en utilisant les options d’enregistrement spécifiées. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Récupère le projet avec le guid spécifié depuis le compte Project Online \ instance de Project Server. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Récupère la liste des projets du magasin 'Working' du compte Project Online actuel \ instance de Project Server. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Récupère les données binaires du projet à des fins de dépannage. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Met à jour le projet existant dans une instance de Project Server\Project Online en utilisant les options d’enregistrement par défaut. Le projet existant sera écrasé. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Met à jour le projet existant dans une instance de Project Server\Project Online en utilisant les options d’enregistrement spécifiées. Le projet existant sera écrasé. |

## Événements

| Nom | Description |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Un événement qui est déclenché lorsque la requête web est envoyée à l’API web de Project Server. |

## Exemples

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


