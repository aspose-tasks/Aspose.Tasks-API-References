---
title: "Enum CustomPropertyType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Properties.CustomPropertyType enum. Vertegenwoordigt een enumeratie van aangepaste eigenschapstypen"
type: docs
weight: 1560
url: /nl/net/aspose.tasks.properties/custompropertytype/
---
## CustomPropertyType enumeration

Stelt een enumeratie van aangepaste eigenschapstypen voor.

```csharp
public enum CustomPropertyType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | De eigenschap heeft geen type. |
| String | `1` | De eigenschap is een tekenreekswaarde. |
| DateTime | `2` | De eigenschap is een datum‑tijdwaarde. |
| Number | `3` | De eigenschap is een geheel getal. |
| Boolean | `4` | De eigenschap is een booleaanse waarde. |

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


