---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定用于处理约束未定义任务的行为。"
type: docs
weight: 329
url: /zh/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

指定用于处理约束未定义任务的行为。
## 字段

| 字段 | 描述 |
| --- | --- |
| [None](#None) | 从 XER 格式加载的默认行为。 |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | 对于具有 'Undefined' 约束的任务，添加类型为 'ConstraintType.StartNoEarlierThan' 且日期 = Start 的约束。 |
### None {#None}
```
public static final int None
```


从 XER 格式加载的默认行为。未采取任何操作。任务约束类型被设置为 'ConstraintType.Undefined'。

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


对于具有 'Undefined' 约束的任务，添加类型为 'ConstraintType.StartNoEarlierThan' 且日期 = Start 的约束。

