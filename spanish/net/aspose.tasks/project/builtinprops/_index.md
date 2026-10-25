---
title: "Project.BuiltInProps"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene la colección de propiedades integradas del proyecto"
type: docs
weight: 100
url: /es/net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

Obtiene la colección de propiedades incorporadas del proyecto.

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
```

## Ejemplos

Muestra cómo leer las meta propiedades del proyecto (API obsoleta).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// las propiedades personalizadas están disponibles a través de la colección tipada
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// las propiedades integradas están disponibles directamente
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// o como un elemento de la colección de propiedades integradas
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### Ver también

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


