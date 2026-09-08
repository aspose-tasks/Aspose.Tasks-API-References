---
title: "Clase ResourceCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ResourceCollection. Representa una colección de objetos Resource"
type: docs
weight: 1770
url: /es/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

Representa una colección de objetos [`Resource`](../resource/).

```csharp
public class ResourceCollection : IList<Resource>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | Obtiene el número de elementos contenidos en ResourceCollection. Int32 de solo lectura. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | Obtiene el proyecto padre del objeto ResourceCollection. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Agrega un nuevo recurso en la última posición de la colección de recursos de un proyecto. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Agrega un nuevo recurso en la última posición de la colección de recursos de un proyecto. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Agrega un nuevo recurso en la posición especificada de la colección de recursos de un proyecto. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | La eliminación directa no está soportada, este método solo lanza NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Devuelve un recurso con el id especificado. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Devuelve un recurso con el Uid especificado. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | Esta es la implementación de sustituto del método Remove de ICollection, que solo lanza NotSupportedException |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | Convierte el objeto ResourceCollection a una lista de objetos [`Resource`](../resource/). |

## Ejemplos

Muestra cómo trabajar con colecciones de recursos.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// agregar recurso vacío
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// agregar recurso con un nombre
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// agregar recurso antes del recurso con ID especificado
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// obtener recurso por id
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// las colecciones de recursos no soportan la operación Clear
// project.Resources.Clear();
// utilice el siguiente ejemplo de código en su lugar
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### Ver también

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


