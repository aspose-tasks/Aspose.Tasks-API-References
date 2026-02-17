---
title: Class Value
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Value class. Represents a value in a value list
type: docs
weight: 2780
url: /net/aspose.tasks/value/
---
## Value class

Represents a value in a value list.

```csharp
public class Value
```

## Constructors

| Name | Description |
| --- | --- |
| [Value](value/)() | Initializes a new instance of the `Value` class. |

## Properties

| Name | Description |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | Gets or sets the actual value if it can be represented as DateTime. Default value is MinValue. |
| [Description](../../aspose.tasks/value/description/) { get; set; } | Gets or sets the description of a value. |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | Gets or sets the actual value which is used to represent Duration. |
| [Id](../../aspose.tasks/value/id/) { get; set; } | Gets or sets the unique identifier of a value across a project. |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | Gets or sets the actual value which is used to represent number or cost value. |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | Gets or sets the phonetic information about custom field name. |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | Gets or sets the actual value which is used to represent Text string. |
| [Val](../../aspose.tasks/value/val/) { get; set; } | Gets or sets the actual value in internal representation. Prefer using strongly typed properties which are listed below. |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | Gets a GUID which identifies this value among others in the entire project. |

## Examples

Shows how to read work with lookup values.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Create an Extended Attribute Definition of Text type
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Add lookup values for the extended attribute definition
textLookup.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1", Phonetic = "Town One" });
textLookup.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2", Phonetic = "Town Two" });

Console.WriteLine("Iterate over text lookup values:");
foreach (var value in textLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("String Value: " + value.StringValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Create an Extended Attribute Definition of Duration type
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// Add lookup values for the extended attribute definition
durationLookup.AddLookupValue(new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours", Phonetic = "Four hours" });
durationLookup.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(8, TimeUnitType.Hour), Description = "1 day", Phonetic = "One day" });
durationLookup.AddLookupValue(new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour", Phonetic = "One hour" });
durationLookup.AddLookupValue(new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days", Phonetic = "Ten days" });

Console.WriteLine("Iterate over duration lookup values:");
foreach (var value in durationLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Duration: " + value.Duration);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Create an Extended Attribute Definition of Date type
var dateLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Date,
    ExtendedAttributeTask.Date1,
    "Custom Date");
dateLookup.AddLookupValue(new Value { Id = 7, DateTimeValue = new DateTime(2020, 4, 27, 8, 0, 0), Description = "Start Date", Phonetic = "Start Date" });

Console.WriteLine("Iterate over date lookup values:");
foreach (var value in dateLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("DateTime Value: " + value.DateTimeValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Create an Extended Attribute Definition of Number type
var numericLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Number,
    ExtendedAttributeTask.Number1,
    "Number of tons");
numericLookup.AddLookupValue(new Value { Id = 8, NumericValue = 10, Description = "10 tons", Phonetic = "Ten tons" });
numericLookup.AddLookupValue(new Value { Id = 9, NumericValue = 20, Description = "20 tons", Phonetic = "Twenty tons" });
numericLookup.AddLookupValue(new Value { Id = 10, NumericValue = 30, Description = "30 tons", Phonetic = "Thirty tons" });

Console.WriteLine("Iterate over numeric lookup values:");
foreach (var value in numericLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Numeric Value: " + value.NumericValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

project.ExtendedAttributes.Add(textLookup);
project.ExtendedAttributes.Add(durationLookup);
project.ExtendedAttributes.Add(dateLookup);
project.ExtendedAttributes.Add(numericLookup);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


