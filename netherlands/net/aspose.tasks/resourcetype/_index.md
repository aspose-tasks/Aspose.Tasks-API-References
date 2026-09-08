---
title: "Enum ResourceType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ResourceType enum. Specificeert het type van een resource"
type: docs
weight: 1800
url: /nl/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Specificeert het type van een resource.

```csharp
public enum ResourceType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Material | `0` | Geeft het type van een materiaalresource aan. |
| Work | `1` | Geeft het type van een werkresource aan. |
| Cost | `2` | Geeft het type van een kostenresource aan. |

## Voorbeelden

Toont hoe te werken met resource-types.

```csharp
var project = new Project();

// voeg een werkresource toe
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// voeg een materiaalresource toe
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// voeg een materiaalresource toe
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// werken met resources: taken maken, resources toewijzen enzovoort...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


