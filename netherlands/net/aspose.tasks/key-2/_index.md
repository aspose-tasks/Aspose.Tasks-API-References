---
title: "Struct KeyTK"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Key2TK struct. Stelt een eigenschapssleutel van een klasse van het opgegeven type voor. Een instantie van deze klasse wordt gebruikt bij het ophalen of instellen van een eigenschap van een container."
type: docs
weight: 930
url: /nl/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

Stelt een eigenschaps-sleutel van een klasse van het opgegeven type voor. Een instantie van deze klasse wordt gebruikt bij het ophalen of instellen van een eigenschap van een container.

```csharp
public struct Key<T, K>
    where K : struct
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type van de eigenschapswaarde. |
| K | Het type van de eigenschapssleutel. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | Haalt de sleutel van de eigenschap op. |

## Voorbeelden

Toont hoe de eigenschap Prj.ActualsInSync gelezen/geschreven kan worden.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


