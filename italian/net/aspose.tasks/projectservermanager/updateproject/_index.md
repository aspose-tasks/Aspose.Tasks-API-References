---
title: ProjectServerManager.UpdateProject
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ProjectServerManager metodo. Aggiorna il progetto esistente nellistanza di Project ServerProject Online utilizzando le opzioni di salvataggio predefinite. Il progetto esistente verrà sovrascritto.
type: docs
weight: 70
url: /it/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Aggiorna il progetto esistente nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio predefinite. Il progetto esistente verrà sovrascritto.

```csharp
public void UpdateProject(Project project)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | Project | Progetto da salvare nell'istanza di Project Server\Project Online. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In caso di errore di comunicazione o errore restituito da un server. |

### Osservazioni

La proprietà del progetto 'project.Get(Prj.Guid)' deve essere un GUID valido di un progetto esistente nell'account Project Server \istanza di Project Online.

### Esempi

In questo esempio il progetto viene caricato dall'account Project Online, modificato e salvato nuovamente nell'account Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

### Guarda anche

* class [Project](../../project/)
* class [ProjectServerManager](../)
* spazio dei nomi [Aspose.Tasks](../../projectservermanager/)
* assemblea [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Aggiorna il progetto esistente nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio specificate. Il progetto esistente verrà sovrascritto.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | Project | Progetto da salvare nell'istanza di Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Istanza di[`ProjectServerSaveOptions`](../../projectserversaveoptions/) classe. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In caso di errore di comunicazione o errore restituito da un server. |

### Osservazioni

saveOptions.ProjectGuid deve essere impostato su un guid di un progetto esistente nell'istanza di Project Server\Project Online.

### Esempi

In questo esempio il progetto viene caricato dall'account Project Online, modificato e salvato nuovamente nell'account Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
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

### Guarda anche

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* spazio dei nomi [Aspose.Tasks](../../projectservermanager/)
* assemblea [Aspose.Tasks](../../../)


