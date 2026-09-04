---
title: "ConstraintType"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定任务开始或结束日期的约束。"
type: docs
weight: 52
url: /zh/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

指定任务开始或完成日期的约束。在导出为 XML 时，未定义的值将从生成的 XML 中删除。
## 字段

| 字段 | 描述 |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Task` 的 `Tsk.Start` 和 `Tsk.Finish` 日期相对于父级 `Tsk.Start` 和 `Tsk.Finish` 日期按 ALAP（尽可能晚）进行调度，并考虑 `Project.TaskLinks`。 |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Task` 的 `Tsk.Start` 和 `Tsk.Finish` 日期相对于父级 `Tsk.Start` 和 `Tsk.Finish` 日期按 ASAP（尽可能早）进行调度，并考虑 `Project.TaskLinks`。 |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | 完成不早于 |
| [FinishNoLaterThan](#FinishNoLaterThan) | 完成不晚于 |
| [MustFinishOn](#MustFinishOn) | 必须在指定日期完成 |
| [MustStartOn](#MustStartOn) | 必须在指定日期开始 |
| [StartNoEarlierThan](#StartNoEarlierThan) | 开始不早于 |
| [StartNoLaterThan](#StartNoLaterThan) | 开始不晚于 |
| [Undefined](#Undefined) | 该值在原始项目文件中未定义。 |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Task` 的 `Tsk.Start` 和 `Tsk.Finish` 日期相对于父级 `Tsk.Start` 和 `Tsk.Finish` 日期按 ALAP（尽可能晚）进行调度，并考虑 `Project.TaskLinks`。

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Task` 的 `Tsk.Start` 和 `Tsk.Finish` 日期相对于父级 `Tsk.Start` 和 `Tsk.Finish` 日期按 ASAP（尽可能早）进行调度，并考虑 `Project.TaskLinks`。

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


完成不早于

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


完成不晚于

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


必须在指定日期完成

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


必须在指定日期开始

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


开始不早于

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


开始不晚于

### Undefined {#Undefined}
```
public static final int Undefined
```


该值在原始项目文件中未定义。

