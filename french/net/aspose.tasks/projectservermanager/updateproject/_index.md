---
title: ProjectServerManager.UpdateProject
second_title: Référence de l'API Aspose.Tasks pour .NET
description: ProjectServerManager méthode. Met à jour le projet existant dans linstance Project ServerProject Online à laide des options denregistrement par défaut. Le projet existant sera écrasé.
type: docs
weight: 70
url: /fr/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Met à jour le projet existant dans l'instance Project Server\Project Online à l'aide des options d'enregistrement par défaut. Le projet existant sera écrasé.

```csharp
public void UpdateProject(Project project)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| project | Project | Projet à enregistrer dans l'instance Project Server\Project Online. |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En cas d'erreur de communication ou d'erreur renvoyée par un serveur. |

### Remarques

La propriété du projet 'project.Get(Prj.Guid)' doit être un guid valide d'un projet qui existe dans le compte Project Server \ instance Project Online.

### Exemples

Dans cet exemple, le projet est chargé à partir du compte Project Online, modifié et enregistré sur le compte Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "mot de passe");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

### Voir également

* class [Project](../../project/)
* class [ProjectServerManager](../)
* espace de noms [Aspose.Tasks](../../projectservermanager/)
* Assemblée [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Met à jour le projet existant dans l'instance Project Server\Project Online à l'aide des options d'enregistrement spécifiées. Le projet existant sera écrasé.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| project | Project | Projet à enregistrer dans l'instance Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Exemple de[`ProjectServerSaveOptions`](../../projectserversaveoptions/) classe. |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En cas d'erreur de communication ou d'erreur renvoyée par un serveur. |

### Remarques

saveOptions.ProjectGuid doit être défini sur un guid d'un projet qui existe sur l'instance Project Server\ Project Online.

### Exemples

Dans cet exemple, le projet est chargé à partir du compte Project Online, modifié et enregistré sur le compte Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "mot de passe");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

### Voir également

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* espace de noms [Aspose.Tasks](../../projectservermanager/)
* Assemblée [Aspose.Tasks](../../../)


