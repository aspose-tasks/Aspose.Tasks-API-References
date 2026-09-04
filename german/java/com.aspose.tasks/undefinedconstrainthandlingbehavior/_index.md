---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for Java API Reference"
description: "Gibt das Verhalten an, das verwendet wird, um Aufgaben mit undefinierten Einschränkungen zu behandeln."
type: docs
weight: 329
url: /de/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

Gibt das Verhalten an, das verwendet wird, um Aufgaben mit undefinierten Einschränkungen zu behandeln.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [None](#None) | Das Standardverhalten beim Laden aus dem XER-Format. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | Einschränkungen mit dem Typ 'ConstraintType.StartNoEarlierThan' und Datum = Start werden für Aufgaben mit der Einschränkung 'Undefined' hinzugefügt. |
### None {#None}
```
public static final int None
```


Das Standardverhalten beim Laden aus dem XER-Format. Es wird keine Aktion durchgeführt. Der Aufgabeneinschränkungstyp wird auf 'ConstraintType.Undefined' gesetzt.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


Einschränkungen mit dem Typ 'ConstraintType.StartNoEarlierThan' und Datum = Start werden für Aufgaben mit der Einschränkung 'Undefined' hinzugefügt.

