---
title: ExtendedAttributeDefinition.Equals
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition method. Returns a flag indicating whether this instance is equal to the specified object
type: docs
weight: 320
url: /net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

Returns a flag indicating whether this instance is equal to the specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | the specified object to compare to this instance. |

### Return Value

a flag indicating whether this instance is equal to the specified object.

## Examples

Shows how to check extended attribute definition equality.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// the equality of calendars is checked against to attribute definition field ids.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### See Also

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


