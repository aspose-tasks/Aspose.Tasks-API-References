---
title: "ResourceCollection.GetById"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceCollection. Devuelve un recurso con el id especificado"
type: docs
weight: 60
url: /es/net/aspose.tasks/resourcecollection/getbyid/
---
## ResourceCollection.GetById method

Devuelve un recurso con el id especificado.

```csharp
public Resource GetById(int id)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| id | Int32 | El id especificado. |

### Valor devuelto

Recurso con el id especificado si está presente; de lo contrario, null.

## Observaciones

Complejidad O(1).

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


