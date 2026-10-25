---
title: "Klasse Value"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Value klasse. Vertegenwoordigt een waarde in een waardelijst"
type: docs
weight: 2800
url: /nl/net/aspose.tasks/value/
---
## Value class

Stelt een waarde in een waardelijst voor.

```csharp
public class Value
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Value](value/)() | Initialiseert een nieuw exemplaar van de `Value` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | Haalt op of stelt de werkelijke waarde in als deze kan worden weergegeven als DateTime. Standaardwaarde is MinValue. |
| [Description](../../aspose.tasks/value/description/) { get; set; } | Haalt op of stelt de beschrijving van een waarde in. |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | Haalt op of stelt de werkelijke waarde in die wordt gebruikt om Duur weer te geven. |
| [Id](../../aspose.tasks/value/id/) { get; set; } | Haalt op of stelt de unieke identifier van een waarde binnen een project in. |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | Haalt op of stelt de werkelijke waarde in die wordt gebruikt om een getal of kostwaarde weer te geven. |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | Haalt op of stelt de fonetische informatie over de naam van een aangepast veld in. |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | Haalt op of stelt de werkelijke waarde in die wordt gebruikt om een tekstreeks weer te geven. |
| [Val](../../aspose.tasks/value/val/) { get; set; } | Haalt op of stelt de werkelijke waarde in in interne representatie. Geef de voorkeur aan het gebruik van sterk getypeerde eigenschappen die hieronder worden vermeld. |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | Haalt een GUID op die deze waarde identificeert tussen andere in het gehele project. |

## Voorbeelden

Toont hoe je werk met lookup-waarden kunt lezen.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Maak een Extended Attribute Definition van het type Tekst
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Voeg lookup-waarden toe voor de extended attribute definition
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

// Maak een Extended Attribute Definition van het type Duur
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// Voeg lookup-waarden toe voor de extended attribute definition
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

// Maak een Extended Attribute Definition van het type Datum
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

// Maak een Extended Attribute Definition van het type Getal
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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


