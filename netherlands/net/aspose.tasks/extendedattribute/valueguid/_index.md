---
title: "ExtendedAttribute.ValueGuid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttribute-eigenschap. Haalt de guid op van een zoekwaarde."
type: docs
weight: 90
url: /nl/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

Haalt de guid van een opzoekwaarde op.

```csharp
public string ValueGuid { get; }
```

## Opmerkingen

Mag niet direct worden ingesteld; gebruik in plaats daarvan ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) om een uitgebreid attribuut met een zoekwaarde te maken.

## Voorbeelden

Toont hoe te werken met een GUID van een uitgebreid attribuut.

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

// uitgebreid attribuut heeft een GUID die is 
// gelijk aan de GUID van de binding 'Value' uit de zoekopdracht
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### Zie ook

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


