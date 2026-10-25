---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for Java API Reference"
description: "Specifica il comportamento usato per gestire le attività con vincoli non definiti."
type: docs
weight: 329
url: /it/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

Specifica il comportamento usato per gestire le attività con vincoli non definiti.
## Campi

| Campo | Descrizione |
| --- | --- |
| [None](#None) | Il comportamento predefinito per il caricamento dal formato XER. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | Vengono aggiunti vincoli con tipo 'ConstraintType.StartNoEarlierThan' e data = Start per le attività con vincolo 'Undefined'. |
### None {#None}
```
public static final int None
```


Il comportamento predefinito per il caricamento dal formato XER. Nessuna azione viene eseguita. Il tipo di vincolo dell'attività è impostato su 'ConstraintType.Undefined'.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


Vengono aggiunti vincoli con tipo 'ConstraintType.StartNoEarlierThan' e data = Start per le attività con vincolo 'Undefined'.

