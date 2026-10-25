---
title: "Clase Property"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Properties.Property. Representa una clase base de una propiedad"
type: docs
weight: 1580
url: /es/net/aspose.tasks.properties/property/
---
## Property class

Representa una clase base de una propiedad.

```csharp
public abstract class Property
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Obtiene un nombre de la propiedad. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Obtiene o establece un valor de la propiedad. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


