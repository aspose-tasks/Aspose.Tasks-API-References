---
title: "Project.CustomProps"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Project. Obtiene la colección de propiedades personalizadas del proyecto"
type: docs
weight: 260
url: /es/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

Obtiene la colección de propiedades personalizadas del proyecto.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
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

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


