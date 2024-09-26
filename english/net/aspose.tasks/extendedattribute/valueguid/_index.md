---
title: ExtendedAttribute.ValueGuid
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttribute property. Gets the guid of a lookup value
type: docs
weight: 90
url: /net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

Gets the guid of a lookup value.

```csharp
public string ValueGuid { get; }
```

## Remarks

Should not be set directly, instead use ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) to create an extended attribute with a lookup value.

## Examples

Shows how to work with an extended attribute GUID.

```csharp
var project = new Project();
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "My lookup cost");
var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));

var value1 = new Value { NumericValue = 10000, Description = "Val 1", Id = 1 };
var value2 = new Value { NumericValue = 25000, Description = "Val 2", Id = 2 };

definition.AddLookupValue(value1);
definition.AddLookupValue(value2);

var attribute = definition.CreateExtendedAttribute(value1);

// extended attribute has a GUID which is 
// equal to GUID of bind 'Value' from the lookup
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### See Also

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


