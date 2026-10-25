---
title: "ConstraintType"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "タスクの開始日または終了日に対する制約を指定します。"
type: docs
weight: 52
url: /ja/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

タスクの開始日または終了日に対する制約を指定します。XML にエクスポートする際、Undefined 値は結果の XML から除外されます。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` と `Tsk.Finish` の `Task` の日付は、親の `Tsk.Start` と `Tsk.Finish` の日付を基準に ALAP でスケジュールされ、`Project.TaskLinks` を考慮します。 |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` と `Tsk.Finish` の `Task` の日付は、親の `Tsk.Start` と `Tsk.Finish` の日付を基準に ASAP でスケジュールされ、`Project.TaskLinks` を考慮します。 |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | 終了はそれ以前にできません |
| [FinishNoLaterThan](#FinishNoLaterThan) | 終了はそれ以降にできません |
| [MustFinishOn](#MustFinishOn) | 必ずこの日に終了する |
| [MustStartOn](#MustStartOn) | 必ずこの日に開始する |
| [StartNoEarlierThan](#StartNoEarlierThan) | 開始はそれ以前にできません |
| [StartNoLaterThan](#StartNoLaterThan) | 開始はそれ以降にできません |
| [Undefined](#Undefined) | 元のプロジェクト ファイルで値が定義されていません。 |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` と `Tsk.Finish` の `Task` の日付は、親の `Tsk.Start` と `Tsk.Finish` の日付を基準に ALAP でスケジュールされ、`Project.TaskLinks` を考慮します。

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` と `Tsk.Finish` の `Task` の日付は、親の `Tsk.Start` と `Tsk.Finish` の日付を基準に ASAP でスケジュールされ、`Project.TaskLinks` を考慮します。

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


終了はそれ以前にできません

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


終了はそれ以降にできません

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


必ずこの日に終了する

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


必ずこの日に開始する

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


開始はそれ以前にできません

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


開始はそれ以降にできません

### Undefined {#Undefined}
```
public static final int Undefined
```


元のプロジェクト ファイルで値が定義されていません。

