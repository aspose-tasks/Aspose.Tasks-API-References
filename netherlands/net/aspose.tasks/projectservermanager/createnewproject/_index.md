---
title: "ProjectServerManager.CreateNewProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerManager-methode. Maakt een nieuw project in een Project Server/Project Online‑instantie met de standaard opslagopties."
type: docs
weight: 30
url: /nl/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Maakt een nieuw project aan in een Project Server\Project Online‑instantie met behulp van de standaard opslagopties.

```csharp
public void CreateNewProject(Project project)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Het project om op te slaan naar de Project Server\Project Online‑instantie. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In geval van een communicatiefout of een fout die door een server wordt geretourneerd. |

## Voorbeelden

In dit voorbeeld wordt het project geladen uit een .mpp‑bestand en opgeslagen in een Project Online‑account.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Toont hoe ProjectServerManager te gebruiken om een nieuw project te maken op Microsoft Project Online.

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

### Zie ook

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Maakt een nieuw project aan in Project Server\Project Online‑instantie met de opgegeven opslagopties.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Het project om op te slaan naar de Project Server\Project Online‑instantie. |
| saveOptions | ProjectServerSaveOptions | Instantie van de [`ProjectServerSaveOptions`](../../projectserversaveoptions/)‑klasse. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In geval van een communicatiefout of een fout die door een server wordt geretourneerd. |

## Voorbeelden

In dit voorbeeld wordt het project geladen uit een .mpp‑bestand en opgeslagen in een Project Online‑account.

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

Toont hoe de Project Server‑manager te gebruiken om een nieuw project te maken met vooraf gedefinieerde opslagopties op Microsoft Project Online.

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

### Zie ook

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


