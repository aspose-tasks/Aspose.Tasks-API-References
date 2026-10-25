---
title: "LevelingOrder"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Definieert de mogelijke waarden van de leveling-volgorde."
type: docs
weight: 143
url: /nl/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Definieert de mogelijke waarden van de leveling-volgorde.
## Velden

| Veld | Beschrijving |
| --- | --- |
| [IdOnly](#IdOnly) | Taken worden vertraagd in oplopende Id-volgorde. |
| [PriorityThenStandard](#PriorityThenStandard) | De prioriteit wordt eerst beschouwd, daarna dezelfde eigenschappen als in Standaard. |
| [Standard](#Standard) | De volgende eigenschappen worden in aanmerking genomen: voorgangerrelaties, totale speling (een taak met een hogere totale speling wordt eerst vertraagd), startdatum, prioriteit. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Taken worden vertraagd in oplopende Id-volgorde.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


De prioriteit wordt eerst beschouwd, daarna dezelfde eigenschappen als in Standaard.

### Standard {#Standard}
```
public static final int Standard
```


De volgende eigenschappen worden in aanmerking genomen: voorgangerrelaties, totale speling (een taak met een hogere totale speling wordt eerst vertraagd), startdatum, prioriteit. Dit is de standaardwaarde.

