---
title: "Clase BuiltInProjectProperty"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Properties.BuiltInProjectProperty. Representa una propiedad incorporada"
type: docs
weight: 1520
url: /es/net/aspose.tasks.properties/builtinprojectproperty/
---
## BuiltInProjectProperty class

Representa una propiedad incorporada.

```csharp
public sealed class BuiltInProjectProperty : Property
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Obtiene un nombre de la propiedad. |
| [Value](../../aspose.tasks.properties/builtinprojectproperty/value/) { get; set; } | Obtiene o establece el valor de la propiedad. (2 propiedades) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Devuelve el valor de la propiedad como cadena. |

## Ejemplos

Muestra cómo leer las propiedades incorporadas del proyecto.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Author: " + project.BuiltInProps.Author);
Console.WriteLine("Category: " + project.BuiltInProps.Category);
Console.WriteLine("Comments: " + project.BuiltInProps.Comments);
Console.WriteLine("Company: " + project.BuiltInProps.Company);
Console.WriteLine("HyperlinkBase: " + project.BuiltInProps.HyperlinkBase);
Console.WriteLine("IsReadOnly: " + project.BuiltInProps.IsReadOnly);
Console.WriteLine("Keywords: " + project.BuiltInProps.Keywords);
Console.WriteLine("Manager: " + project.BuiltInProps.Manager);
Console.WriteLine("Subject: " + project.BuiltInProps.Subject);
Console.WriteLine("Title: " + project.BuiltInProps.Title);
Console.WriteLine();

// iterar sobre la colección de propiedades incorporadas
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### Ver también

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


