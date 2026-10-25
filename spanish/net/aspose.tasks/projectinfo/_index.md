---
title: "Clase ProjectInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ProjectInfo. Información breve sobre el proyecto publicado disponible en Project Online"
type: docs
weight: 1470
url: /es/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Información breve sobre el proyecto publicado disponible en Project Online.

```csharp
public sealed class ProjectInfo
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ProjectInfo](projectinfo/)() | Inicializa una nueva instancia de la clase `ProjectInfo`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Obtiene la fecha y hora en que se creó el proyecto. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Obtiene la descripción del proyecto. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Obtiene el identificador único del proyecto. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Obtiene un valor que indica si el proyecto está reservado. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Obtiene la fecha más reciente en que se publicó el proyecto. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Obtiene la fecha más reciente en que se guardó el proyecto. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Obtiene el nombre del proyecto. |

## Ejemplos

Muestra cómo leer información sobre proyectos desde Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// leer la información del proyecto
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


