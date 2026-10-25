---
title: "ProjectServerManager.CreateNewProject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectServerManager. Crea un nuevo proyecto en la instancia de Project Server/Project Online usando las opciones de guardado predeterminadas."
type: docs
weight: 30
url: /es/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Crea un nuevo proyecto en la instancia Project Server\Project Online usando las opciones de guardado predeterminadas.

```csharp
public void CreateNewProject(Project project)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | Project | El proyecto a guardar en la instancia de Project Server\\Project Online. |

### Excepciones

| excepción | condición |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En caso de error de comunicación o error devuelto por un servidor. |

## Ejemplos

En este ejemplo, el proyecto se carga desde un archivo .mpp y se guarda en la cuenta de Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Muestra cómo usar ProjectServerManager para crear un nuevo proyecto en Microsoft Project Online.

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

### Ver también

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Crea un nuevo proyecto en la instancia de Project Server\\Project Online usando las opciones de guardado especificadas.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | Project | El proyecto a guardar en la instancia de Project Server\\Project Online. |
| saveOptions | ProjectServerSaveOptions | Instancia de la clase [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Excepciones

| excepción | condición |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | En caso de error de comunicación o error devuelto por un servidor. |

## Ejemplos

En este ejemplo, el proyecto se carga desde un archivo .mpp y se guarda en la cuenta de Project Online.

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

Muestra cómo usar el administrador de Project Server para crear un nuevo proyecto con opciones de guardado predefinidas en Microsoft Project Online.

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

### Ver también

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


