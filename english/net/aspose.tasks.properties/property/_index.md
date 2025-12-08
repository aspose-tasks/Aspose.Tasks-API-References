---
title: Class Property
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Properties.Property class. Represents a base class of a property
type: docs
weight: 1550
url: /net/aspose.tasks.properties/property/
---
## Property class

Represents a base class of a property.

```csharp
public abstract class Property
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Gets a name of the property. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Gets or sets a value of the property. |

## Methods

| Name | Description |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Returns the property value as string. |

## Examples

Shows how to read project builtin properties.

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

// iterate over built-in property collection
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### See Also

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


