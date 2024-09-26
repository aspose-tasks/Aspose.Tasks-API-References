---
title: Resource.ExtendedAttributes
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets the values of an extended attribute
type: docs
weight: 320
url: /net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Gets the values of an extended attribute.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Remarks

Two pieces of data are necessary - a pointer back to the extended attribute table which is specified either by the unique ID or the Field ID, and the value which is specified either with the value, or a pointer back to the value list.

## Examples

Shows how to add resource extended attributes.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Define extended attribute
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Create extended attribute and set its value
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Add a new resource and its extended attribute   
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


