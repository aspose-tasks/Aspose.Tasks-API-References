---
title: UndefinedConstraintHandlingBehavior
second_title: Aspose.Tasks for Java API Reference
description: Specifies the behavior used to handle tasks with undefined constraints.
type: docs
weight: 326
url: /java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

Specifies the behavior used to handle tasks with undefined constraints.
## Fields

| Field | Description |
| --- | --- |
| [None](#None) | The default behavior for loading from XER format. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | Constraints with type 'ConstraintType.StartNoEarlierThan' and date = Start are added for tasks with 'Undefined' constraint. |
### None {#None}
```
public static final int None
```


The default behavior for loading from XER format. No action is taken. A task constraint type is set to 'ConstraintType.Undefined'.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


Constraints with type 'ConstraintType.StartNoEarlierThan' and date = Start are added for tasks with 'Undefined' constraint.

