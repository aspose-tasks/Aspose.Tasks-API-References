---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen af te handelen."
type: docs
weight: 329
url: /nl/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen af te handelen.
## Velden

| Veld | Beschrijving |
| --- | --- |
| [None](#None) | Het standaardgedrag voor het laden vanuit XER-indeling. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | Beperkingen met type 'ConstraintType.StartNoEarlierThan' en datum = Start worden toegevoegd voor taken met de beperking 'Undefined'. |
### None {#None}
```
public static final int None
```


Het standaardgedrag voor het laden vanuit XER-indeling. Er wordt geen actie ondernomen. Een taakbeperkingstype wordt ingesteld op 'ConstraintType.Undefined'.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


Beperkingen met type 'ConstraintType.StartNoEarlierThan' en datum = Start worden toegevoegd voor taken met de beperking 'Undefined'.

