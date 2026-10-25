---
title: "LevelingOrder"
second_title: "Aspose.Tasks for Java API Reference"
description: "Definiert die möglichen Werte der Ausgleichsreihenfolge."
type: docs
weight: 143
url: /de/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Definiert die möglichen Werte der Ausgleichsreihenfolge.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [IdOnly](#IdOnly) | Aufgaben werden in aufsteigender Id-Reihenfolge verzögert. |
| [PriorityThenStandard](#PriorityThenStandard) | Die Priorität wird zuerst berücksichtigt, dann die gleichen Eigenschaften wie im Standard. |
| [Standard](#Standard) | Die folgenden Eigenschaften werden berücksichtigt: Vorgängerbeziehungen, Gesamtspielraum (eine Aufgabe mit höherem Gesamtspielraum wird zuerst verzögert), Startdatum, Priorität. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Aufgaben werden in aufsteigender Id-Reihenfolge verzögert.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


Die Priorität wird zuerst berücksichtigt, dann die gleichen Eigenschaften wie im Standard.

### Standard {#Standard}
```
public static final int Standard
```


Die folgenden Eigenschaften werden berücksichtigt: Vorgängerbeziehungen, Gesamtspielraum (eine Aufgabe mit höherem Gesamtspielraum wird zuerst verzögert), Startdatum, Priorität. Dies ist der Standardwert.

