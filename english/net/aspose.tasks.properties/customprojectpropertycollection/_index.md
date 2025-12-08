---
title: Class CustomProjectPropertyCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Properties.CustomProjectPropertyCollection class. Represents a collection of custom project properties
type: docs
weight: 1520
url: /net/aspose.tasks.properties/customprojectpropertycollection/
---
## CustomProjectPropertyCollection class

Represents a collection of custom project properties.

```csharp
public sealed class CustomProjectPropertyCollection : PropertyKeyedCollection<CustomProjectProperty>
```

## Constructors

| Name | Description |
| --- | --- |
| [CustomProjectPropertyCollection](customprojectpropertycollection/)() | Initializes a new instance of the `CustomProjectPropertyCollection` class. |

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| override [IsReadOnly](../../aspose.tasks.properties/customprojectpropertycollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(CustomProjectProperty) |  |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add)(string, bool) | Creates a new custom property. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_2)(string, DateTime) | Creates a new custom property. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_1)(string, double) | Creates a new custom property. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_3)(string, string) | Creates a new custom property. |
| [Clear](../../aspose.tasks.properties/customprojectpropertycollection/clear/)() | Clears the PropertyCollection. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |
| [Remove](../../aspose.tasks.properties/customprojectpropertycollection/remove/)(string) | Removes a property with the specified name from the collection. |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [CustomProjectProperty](../customprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


