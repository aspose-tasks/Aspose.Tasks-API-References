---
title: "Enum UndefinedConstraintHandlingBehavior"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.UndefinedConstraintHandlingBehavior. Specifica il comportamento utilizzato per gestire le attività con vincoli non definiti"
type: docs
weight: 2630
url: /it/net/aspose.tasks/undefinedconstrainthandlingbehavior/
---
## UndefinedConstraintHandlingBehavior enumeration

Specifica il comportamento utilizzato per gestire le attività con vincoli non definiti.

```csharp
public enum UndefinedConstraintHandlingBehavior
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Il comportamento predefinito per il caricamento dal formato XER. Non viene eseguita alcuna azione. Il tipo di vincolo di un'attività è impostato su 'ConstraintType.Undefined'. |
| SubstituteWithStartNoEarlierThan | `1` | I vincoli con tipo 'ConstraintType.StartNoEarlierThan' e data = Start vengono aggiunti per le attività con vincolo 'Undefined'. |

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


