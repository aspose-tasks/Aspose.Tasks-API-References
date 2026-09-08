---
title: "Klasse OutlineValueCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineValueCollection klasse. Stelt een collectie van OutlineValue-objecten voor."
type: docs
weight: 1220
url: /nl/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

Stelt een collectie van [`OutlineValue`](../outlinevalue/) objecten voor.

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | Retourneert of stelt het element in op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | Bepaalt de index van het opgegeven item in deze collectie. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | Voegt het opgegeven item in op de opgegeven index. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | Verwijdert een item op de opgegeven index. |

## Voorbeelden

Toont hoe te werken met outline-waardecollecties.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// waardecollecties wissen
foreach (var outlineCode in project.OutlineCodes)
{
    // outline-masks wissen
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// waarde bijwerken via indextoegang
codeDefinition.Values[0].Value = "654321";

// itereren over outline-waarden
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// werken met outline-waarden
// ...

// verwijder een waarde indien nodig
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// voeg een waarde in op de startpositie
codeDefinition.Values.Insert(0, value);

// controleer de positie van de ingevoegde waarde
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// werken met outline-waarden
// ...

// verwijder de laatste waarde uit de collectie
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// men kan een andere outline-code-definitie maken
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// en vervolgens outline-waarden kopiëren
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Zie ook

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


