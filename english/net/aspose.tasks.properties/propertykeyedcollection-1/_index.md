---
title: Class PropertyKeyedCollectionT
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Properties.PropertyKeyedCollection1T class. A base class of collection of properties
type: docs
weight: 1570
url: /net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

A base class of collection of properties.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| Parameter | Description |
| --- | --- |
| T | The type of property. |

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | Gets the number of properties in the collection. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | Gets the Property associated with the specified key. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | Gets the collection of all property names. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | Creates a new custom property. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | Determines whether the [`PropertyCollection`](../propertycollection-1/) contains a property with the specified name. |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


