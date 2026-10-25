---
title: "Enum EarnedValueMethodType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.EarnedValueMethodType enum. Specificeert de methode die wordt gebruikt voor het berekenen van verdiende waarde"
type: docs
weight: 480
url: /nl/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Specificeert de methode die wordt gebruikt voor het berekenen van verdiende waarde.

```csharp
public enum EarnedValueMethodType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Het veld was niet gedefinieerd in het oorspronkelijke projectbestand. |
| PercentComplete | `0` | Percentage voltooid |
| PhysicalPercentComplete | `1` | Fysiek percentage voltooid |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe de methode die wordt gebruikt voor het berekenen van verdiende waarde (EarnedValueMethodType.PercentComplete) te specificeren.

```csharp
var project = new Project(DataDir + "Project2.mpp");
// stel het earned value-methode type in op 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// werken met het project...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


