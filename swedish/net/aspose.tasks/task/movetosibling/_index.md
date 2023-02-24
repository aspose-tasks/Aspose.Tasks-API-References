---
title: Task.MoveToSibling
second_title: Aspose.Tasks för .NET API-referens
description: Task metod. Flyttar den aktuella uppgiften till samma dispositionsnivå före den angivna uppgiften. Om ParentProject.CalculationMode är None bör användaren anropa Project.Recalculate efter att ha använt denna metod Det kommer att omschemalägga alla projektuppgifter start/slutdatum ställer in tidigt/ sena datum och beräkna de beroende fälten såsom slacks work and cost fields disposition levels. Om ParentProject.CalculationMode är manuell kommer metoden endast att beräkna uppgiftsid dispositionsnivå och dispositionsnummer automatiskt. Om ParentProject.CalculationMode är Automatic metoden schemalägger alla projekts uppgifter automatiskt start/slutdatum sätter tidiga/sena datum beräknar slack arbets och kostnadsfält räknar om id och dispositionsnivåer.
type: docs
weight: 1370
url: /sv/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Flyttar den aktuella uppgiften till samma dispositionsnivå före den angivna uppgiften. Om ParentProject.CalculationMode är None bör användaren anropa Project.Recalculate() efter att ha använt denna metod (Det kommer att omschemalägga alla projektuppgifter (start-/slutdatum, ställer in tidigt/ sena datum) och beräkna de beroende fälten såsom slacks, work and cost fields, disposition levels). Om ParentProject.CalculationMode är manuell kommer metoden endast att beräkna uppgifts-id, dispositionsnivå och dispositionsnummer automatiskt. Om ParentProject.CalculationMode är Automatic metoden schemalägger alla projekts uppgifter automatiskt (start-/slutdatum, sätter tidiga/sena datum, beräknar slack-, arbets- och kostnadsfält, räknar om id och dispositionsnivåer).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| beforeTask | Task | Uppgift innan den aktuella uppgiften kommer att infogas. |

### Se även

* class [Task](../)
* namnutrymme [Aspose.Tasks](../../task/)
* hopsättning [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Flyttar den aktuella uppgiften till samma dispositionsnivå före en uppgift med det angivna Id. If ParentProject.CalculationMode is None bör användaren anropa Project.Recalculate() efter att ha använt den här metoden (Det kommer att schemalägga alla projektuppgifter (start-/slutdatum, sätter tidiga/sena datum) och beräkna de beroende fälten såsom slacks, work and cost fields, disposition levels). Om ParentProject.CalculationMode är manuell kommer metoden endast att beräkna uppgifts-id, dispositionsnivå och dispositionsnummer automatiskt. If ParentProject. CalculationMode är Automatisk metoden schemalägger alla projekts uppgifter automatiskt (start-/slutdatum, anger tidiga/sena datum, beräknar slacks, arbets- och kostnadsfält, räknar om id och dispositionsnivåer).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| beforeTaskId | Int32 | ID ([`Id`](../../tsk/id/)) för en uppgift innan den aktuella uppgiften kommer att infogas. |

### Se även

* class [Task](../)
* namnutrymme [Aspose.Tasks](../../task/)
* hopsättning [Aspose.Tasks](../../../)


