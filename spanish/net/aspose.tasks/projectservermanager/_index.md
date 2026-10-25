---
title: "Clase ProjectServerManager"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.ProjectServerManager class. La clase que proporciona los métodos para leer y realizar operaciones en proyectos en la cuenta especificada de Project Online o en la instancia onpremise especificada de Project Server. Se admiten versiones de Project Server 2016 y 2019."
type: docs
weight: 1500
url: /es/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

La clase que proporciona los métodos para leer y realizar operaciones en proyectos en la cuenta especificada de Project Online o en la instancia especificada local de Project Server (se admiten las versiones 2016 y 2019 de Project Server).

```csharp
public sealed class ProjectServerManager
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Inicializa una nueva instancia de la clase `ProjectServerManager`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Crea un nuevo proyecto en la instancia Project Server\Project Online usando las opciones de guardado predeterminadas. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Crea un nuevo proyecto en la instancia de Project Server\\Project Online usando las opciones de guardado especificadas. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Obtiene el proyecto con el GUID especificado de la cuenta de Project Online \\ instancia de Project Server. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Obtiene la lista de proyectos del almacén 'Working' de la cuenta actual de Project Online \\ instancia de Project Server. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Obtiene los datos binarios del proyecto con fines de solución de problemas. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Actualiza el proyecto existente en la instancia de Project Server\\Project Online usando las opciones de guardado predeterminadas. El proyecto existente será sobrescrito. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Actualiza el proyecto existente en la instancia de Project Server\\Project Online usando las opciones de guardado especificadas. El proyecto existente será sobrescrito. |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Un evento que se genera cuando la solicitud web se envía a la API web de Project Server. |

## Ejemplos

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


