---
title: ResourceAssignment.ExtendedAttributes
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment property. Gets or sets an instance of the ExtendedAttributeCollection class for this object
type: docs
weight: 250
url: /net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Gets or sets an instance of the ExtendedAttributeCollection class for this object.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Remarks

Reading supported for XML format only.

## Examples

Shows how to add extended attributes for an assignment.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Assign resource "1 TRG: Trade Group" to the "TASK 1" by creating a ResourceAssignment object.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Create custom attribute definition with lookup.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// This value can be seen in "Resource usage" view of MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### See Also

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


