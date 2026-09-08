---
title: "Enum CostAccrualType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CostAccrualType enum. Specificeert het type van een accrual‑kosten."
type: docs
weight: 350
url: /nl/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

Specificeert het type van een opbouwkost.

```csharp
public enum CostAccrualType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Geeft aan dat een ongedefinieerde waarde betekent dat het veld niet gedefinieerd was in het oorspronkelijke projectbestand. |
| Start | `0` | Geeft het Start‑kosten‑accrualtype aan. |
| Prorated | `1` | Geeft het Prorated‑kosten‑accrualtype aan. |
| End | `2` | Geeft het End‑kosten‑accrualtype aan. |
| Invalid | `3` | Geeft het Invalid‑kosten‑accrualtype aan. |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe en wanneer standaard- en overurenkosten van resources moeten worden gefactureerd, of geaccrueerd (accrual‑methode: Bepaalt wanneer de kosten voor een resource ontstaan en wanneer werkelijke kosten aan een project worden gefactureerd. Je kunt kosten laten ontstaan bij de start [Start] of het einde [End] van een taak of ze tijdens de taak proraten [Prorated].), naar de kosten van een taak (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// stel kosten‑accrualtype in
// als je de End‑optie selecteert, worden kosten niet geaccrueerd totdat het resterende werk nul is.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// werken met het project...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


