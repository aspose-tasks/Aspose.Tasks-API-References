---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for Java API-referens"
description: "Anger beteendet som används för att hantera uppgifter med odefinierade begränsningar."
type: docs
weight: 329
url: /sv/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

Anger beteendet som används för att hantera uppgifter med odefinierade begränsningar.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [None](#None) | Standardbeteendet för inläsning från XER-format. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | Begränsningar med typen 'ConstraintType.StartNoEarlierThan' och datum = Start läggs till för uppgifter med 'Undefined'-begränsning. |
### None {#None}
```
public static final int None
```


Standardbeteendet för inläsning från XER-format. Ingen åtgärd vidtas. En uppgiftsbegränsningstyp sätts till 'ConstraintType.Undefined'.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


Begränsningar med typen 'ConstraintType.StartNoEarlierThan' och datum = Start läggs till för uppgifter med 'Undefined'-begränsning.

