---
title: "ProjectInfo.LastSavedDate"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ProjectInfo propiedad. Obtiene la fecha más reciente en que se guardó el proyecto"
type: docs
weight: 70
url: /es/net/aspose.tasks/projectinfo/lastsaveddate/
---
## ProjectInfo.LastSavedDate property

Obtiene la fecha más reciente en que se guardó el proyecto.

```csharp
public DateTime LastSavedDate { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


