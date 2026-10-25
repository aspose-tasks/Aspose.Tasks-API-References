---
title: "Struct GenericPropertyTKey"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Properties.GenericProperty1TKey struct. Vertegenwoordigt een container‑eigenschap"
type: docs
weight: 1570
url: /nl/net/aspose.tasks.properties/genericproperty-1/
---
## GenericProperty&lt;TKey&gt; structure

Stelt een container‑eigenschap voor.

```csharp
public struct GenericProperty<TKey>
    where TKey : struct
```

| Parameter | Beschrijving |
| --- | --- |
| TKey | Het type van de eigenschapswaarde. |

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [GenericProperty](genericproperty/)(string) | Initialiseert een nieuw exemplaar van de `GenericProperty` struct. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Name](../../aspose.tasks.properties/genericproperty-1/name/) { get; } | Haalt de naam van de eigenschap op. |
| [Value](../../aspose.tasks.properties/genericproperty-1/value/) { get; } | Haalt een waarde van de eigenschap op. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


