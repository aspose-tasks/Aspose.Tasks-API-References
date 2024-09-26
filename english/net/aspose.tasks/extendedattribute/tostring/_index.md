---
title: ExtendedAttribute.ToString
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttribute method. Returns short string representation of an extended attribute
type: docs
weight: 110
url: /net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Returns short string representation of an extended attribute.

```csharp
public override string ToString()
```

### Return Value

The string representation of the extended attribute.

## Examples

Shows how to read extended attributes.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Read extended attributes for tasks
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // read common info about extended attribute
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### See Also

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


