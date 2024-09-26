---
title: Property.Value
second_title: Aspose.Tasks for .NET API Reference
description: Property property. Gets or sets a value of the property
type: docs
weight: 20
url: /net/aspose.tasks.properties/property/value/
---
## Property.Value property

Gets or sets a value of the property.

```csharp
public object Value { get; set; }
```

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

* class [Property](../)
* namespace [Aspose.Tasks.Properties](../../property/)
* assembly [Aspose.Tasks](../../../)


