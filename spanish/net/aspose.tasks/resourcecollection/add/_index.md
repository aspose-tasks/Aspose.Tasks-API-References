---
title: "ResourceCollection.Add"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceCollection. Añade un nuevo recurso en la última posición de la colección de recursos de un proyecto"
type: docs
weight: 40
url: /es/net/aspose.tasks/resourcecollection/add/
---
## Add() {#add}

Agrega un nuevo recurso en la última posición de la colección de recursos de un proyecto.

```csharp
public Resource Add()
```

### Valor devuelto

Recurso añadido.

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

---

## Add(string) {#add_1}

Agrega un nuevo recurso en la última posición de la colección de recursos de un proyecto.

```csharp
public Resource Add(string resourceName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| resourceName | Cadena | Nombre de un recurso. |

### Valor devuelto

Recurso añadido.

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

---

## Add(string, int) {#add_2}

Agrega un nuevo recurso en la posición especificada de la colección de recursos de un proyecto.

```csharp
public Resource Add(string resourceName, int beforeResourceId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| resourceName | Cadena | Nombre de un recurso. |
| beforeResourceId | Int32 | Posición del recurso anterior en la colección de recursos del proyecto. |

### Valor devuelto

Recurso añadido.

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


