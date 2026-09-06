---
title: "ExtendedAttribute.ValueGuid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ExtendedAttribute. Obtient le guid d'une valeur de recherche"
type: docs
weight: 90
url: /fr/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

Obtient le guid d'une valeur de recherche.

```csharp
public string ValueGuid { get; }
```

## Remarques

Ne doit pas être défini directement, utilisez plutôt ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) pour créer un attribut étendu avec une valeur de recherche.

## Exemples

Montre comment travailler avec un GUID d'attribut étendu.

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

// l'attribut étendu possède un GUID qui est 
// égal au GUID de la liaison 'Value' provenant de la recherche
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### Voir aussi

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


