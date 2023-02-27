---
title: Project.Recalculate
second_title: Aspose.Tasks för .NET API-referens
description: Project metod. Omschemalägger alla projektuppgifterID dispositionsnivåer start/slutdatum anger tidiga/sena datum beräknar slacks arbete och kostnadsfält.
type: docs
weight: 1120
url: /sv/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Omschemalägger alla projektuppgifter-ID, dispositionsnivåer, start-/slutdatum, anger tidiga/sena datum, beräknar slacks, arbete och kostnadsfält.

```csharp
public void Recalculate()
```

### Se även

* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Omschemalägger alla projektuppgifter-ID, dispositionsnivåer, start-/slutdatum, ställer in tidiga/sena datum, beräknar slack-, arbete- och kostnadsfält med valfri validering.

```csharp
public void Recalculate(bool validate)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| validate | Boolean | Om sant kommer valideringen av omräkningen att utföras. Vilka data valideras: För närvarande implementeras endast grundläggande validering av uppgifts- och uppgiftslänkdatumintervall. Uppgiftens datumintervall (t.ex. ActualStart - ActualFinish, EarlyFinish - etc. ) samt datum för uppgiftslänkar kommer att kontrolleras mot datumkriterierna där startdatumet är mindre eller lika med slutdatumet. Om något av villkoren som beskrivs ovan misslyckas,[`RecalculationValidationException`](../../recalculationvalidationexception/)kommer att kastas. |

### Se även

* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)


