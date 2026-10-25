---
title: "Clase BuiltInProjectPropertyCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Properties.BuiltInProjectPropertyCollection. Representa una colección de propiedades incorporadas del proyecto"
type: docs
weight: 1530
url: /es/net/aspose.tasks.properties/builtinprojectpropertycollection/
---
## BuiltInProjectPropertyCollection class

Representa una colección de propiedades de proyecto incorporadas.

```csharp
public sealed class BuiltInProjectPropertyCollection : 
    PropertyKeyedCollection<BuiltInProjectProperty>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Author](../../aspose.tasks.properties/builtinprojectpropertycollection/author/) { get; set; } | Obtiene o establece el autor de un proyecto. |
| [Category](../../aspose.tasks.properties/builtinprojectpropertycollection/category/) { get; set; } | Obtiene o establece la categoría de un proyecto. |
| [Comments](../../aspose.tasks.properties/builtinprojectpropertycollection/comments/) { get; set; } | Obtiene o establece los comentarios de un proyecto. |
| [Company](../../aspose.tasks.properties/builtinprojectpropertycollection/company/) { get; set; } | Obtiene o establece la empresa de un proyecto. |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| [HyperlinkBase](../../aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/) { get; set; } | Obtiene o establece la base de hipervínculo de un proyecto. |
| override [IsReadOnly](../../aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Keywords](../../aspose.tasks.properties/builtinprojectpropertycollection/keywords/) { get; set; } | Obtiene o establece las palabras clave de un proyecto. |
| [Manager](../../aspose.tasks.properties/builtinprojectpropertycollection/manager/) { get; set; } | Obtiene o establece el gestor de un proyecto. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |
| [Subject](../../aspose.tasks.properties/builtinprojectpropertycollection/subject/) { get; set; } | Obtiene o establece el asunto de un proyecto. |
| [Title](../../aspose.tasks.properties/builtinprojectpropertycollection/title/) { get; set; } | Obtiene o establece el título de un proyecto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(BuiltInProjectProperty) |  |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [BuiltInProjectProperty](../builtinprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


