---
title: Class CustomProjectProperty
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Properties.CustomProjectProperty class. Represents a custom property
type: docs
weight: 1520
url: /net/aspose.tasks.properties/customprojectproperty/
---
## CustomProjectProperty class

Represents a custom property.

```csharp
public sealed class CustomProjectProperty : Property
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Gets a name of the property. |
| [Type](../../aspose.tasks.properties/customprojectproperty/type/) { get; } | Gets a type of the property. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Gets or sets a value of the property. |

## Methods

| Name | Description |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Returns the property value as string. |

## Examples

Shows how to work with custom project property collections.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// lets add new custom properties
// collection support Boolean, DateTime, Double, String types
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// custom properties are available through the typed collection
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// get a custom property value
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// iterate over names of custom properties
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// one can delete a value by string key
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// or one can clear collection completely
project.CustomProps.Clear();
```

### See Also

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


