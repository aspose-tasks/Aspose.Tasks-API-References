---
title: ExtendedAttributeDefinition.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition method. Returns a hash code for the instance of the ExtendedAttributeDefinition class
type: docs
weight: 330
url: /net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

Returns a hash code for the instance of the [`ExtendedAttributeDefinition`](../) class.

```csharp
public override int GetHashCode()
```

### Return Value

a hash code for this object.

## Examples

Shows how to get a hash code of a extended attribute definition.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// the hash code of a extended attribute definition is equal to a field id.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### See Also

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


