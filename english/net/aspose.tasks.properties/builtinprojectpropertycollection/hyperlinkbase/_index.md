---
title: BuiltInProjectPropertyCollection.HyperlinkBase
second_title: Aspose.Tasks for .NET API Reference
description: BuiltInProjectPropertyCollection property. Gets or sets the hyperlink base of a project
type: docs
weight: 50
url: /net/aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/
---
## BuiltInProjectPropertyCollection.HyperlinkBase property

Gets or sets the hyperlink base of a project.

```csharp
public string HyperlinkBase { get; set; }
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

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


