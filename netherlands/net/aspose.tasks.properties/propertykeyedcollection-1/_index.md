---
title: "Klasse PropertyKeyedCollectionT"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Properties.PropertyKeyedCollection1T klasse. Een basisklasse van een verzameling eigenschappen"
type: docs
weight: 1600
url: /nl/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

Een basisklasse van een verzameling eigenschappen.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type van de eigenschap. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | Haalt het aantal eigenschappen in de verzameling op. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | Haalt de Property op die bij de opgegeven sleutel hoort. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | Haalt de verzameling van alle eigenschapsnamen op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | Maakt een nieuwe aangepaste eigenschap. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | Bepaalt of de [`PropertyCollection`](../propertycollection-1/) een eigenschap met de opgegeven naam bevat. |

## Voorbeelden

Toont hoe te werken met aangepaste project‑eigenschapcollecties.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// Laten we nieuwe aangepaste eigenschappen toevoegen
// Collectie ondersteunt Boolean-, DateTime-, Double- en String‑typen
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// Aangepaste eigenschappen zijn beschikbaar via de getypeerde collectie
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// Haal een aangepaste eigenschapswaarde op
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// Itereer over de namen van aangepaste eigenschappen
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// Je kunt een waarde verwijderen met een string‑sleutel
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// of men kan de collectie volledig wissen
project.CustomProps.Clear();
```

### Zie ook

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


