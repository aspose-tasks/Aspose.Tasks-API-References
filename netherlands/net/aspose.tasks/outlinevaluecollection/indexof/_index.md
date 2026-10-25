---
title: "OutlineValueCollection.IndexOf"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OutlineValueCollection methode. Bepaalt de index van het opgegeven item in deze collectie"
type: docs
weight: 90
url: /nl/net/aspose.tasks/outlinevaluecollection/indexof/
---
## OutlineValueCollection.IndexOf method

Bepaalt de index van het opgegeven item in deze collectie.

```csharp
public int IndexOf(OutlineValue item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | OutlineValue | het opgegeven item om te vinden in deze collectie. |

### Retourwaarde

de index van het opgegeven item indien gevonden; anders -1.

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

* class [OutlineValue](../../outlinevalue/)
* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


