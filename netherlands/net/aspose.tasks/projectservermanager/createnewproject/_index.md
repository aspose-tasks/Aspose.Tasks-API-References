---
title: CreateNewProject
second_title: Aspose.Tasks voor .NET API-referentie
description: Maakt nieuw project in Project ServerProject Onlineinstantie met standaard opslagopties.
type: docs
weight: 30
url: /nl/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Maakt nieuw project in Project Server\Project Online-instantie met standaard opslagopties.

```csharp
public void CreateNewProject(Project project)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Het project dat moet worden opgeslagen in de Project Server\Project Online-instantie. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In geval van communicatiefout of fout geretourneerd door een server. |

### Voorbeelden

In dit voorbeeld wordt het project geladen vanuit het .mpp-bestand en opgeslagen in het Project Online-account.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "jjjjj@xxxxxxx.onmicrosoft.com", "wachtwoord");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

### Zie ook

* class [Project](../../project/)
* class [ProjectServerManager](../)
* naamruimte [Aspose.Tasks](../../projectservermanager/)
* montage [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Maakt een nieuw project in de Project Server\Project Online-instantie met behulp van de opgegeven opslagopties.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Het project dat moet worden opgeslagen in de Project Server\Project Online-instantie. |
| saveOptions | ProjectServerSaveOptions | Instantie van[`ProjectServerSaveOptions`](../../projectserversaveoptions/) klas. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In geval van communicatiefout of fout geretourneerd door een server. |

### Voorbeelden

In dit voorbeeld wordt het project geladen vanuit het .mpp-bestand en opgeslagen in het Project Online-account.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "jjjjj@xxxxxxx.onmicrosoft.com", "wachtwoord");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

### Zie ook

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* naamruimte [Aspose.Tasks](../../projectservermanager/)
* montage [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->