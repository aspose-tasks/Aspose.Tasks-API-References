---
title: CustomProjectPropertyCollection.Remove
second_title: Aspose.Tasks for .NET API Reference
description: CustomProjectPropertyCollection method. Removes a property with the specified name from the collection
type: docs
weight: 50
url: /net/aspose.tasks.properties/customprojectpropertycollection/remove/
---
## CustomProjectPropertyCollection.Remove method

Removes a property with the specified name from the collection.

```csharp
public bool Remove(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

### Return Value

True if the element is successfully found and removed; otherwise, false.

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

* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


