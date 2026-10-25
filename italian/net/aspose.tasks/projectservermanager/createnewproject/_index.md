---
title: "ProjectServerManager.CreateNewProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectServerManager. Crea un nuovo progetto nell'istanza Project Server/Project Online usando le opzioni di salvataggio predefinite"
type: docs
weight: 30
url: /it/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Crea un nuovo progetto nell'istanza Project Server\Project Online utilizzando le opzioni di salvataggio predefinite.

```csharp
public void CreateNewProject(Project project)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| progetto | Project | Il progetto da salvare nell'istanza Project Server\Project Online. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In caso di errore di comunicazione o di errore restituito da un server. |

## Esempi

In questo esempio il progetto viene caricato da un file .mpp e salvato nell'account di Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Mostra come utilizzare ProjectServerManager per creare un nuovo progetto su Microsoft Project Online.

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

### Vedi anche

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Crea un nuovo progetto nell'istanza di Project Server\Project Online utilizzando le opzioni di salvataggio specificate.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| progetto | Project | Il progetto da salvare nell'istanza Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Istanza della classe [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In caso di errore di comunicazione o di errore restituito da un server. |

## Esempi

In questo esempio il progetto viene caricato da un file .mpp e salvato nell'account di Project Online.

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

Mostra come utilizzare il gestore di Project Server per creare un nuovo progetto con opzioni di salvataggio predefinite su Microsoft Project Online.

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

### Vedi anche

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


