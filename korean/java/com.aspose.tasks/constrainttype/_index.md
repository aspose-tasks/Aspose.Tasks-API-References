---
title: "ConstraintType"
second_title: "Aspose.Tasks for Java API Reference"
description: "작업의 시작 또는 종료 날짜에 대한 제약을 지정합니다."
type: docs
weight: 52
url: /ko/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

작업의 시작 또는 완료 날짜에 대한 제약을 지정합니다. XML로 내보낼 때 Undefined 값은 결과 XML에서 제거됩니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Task`의 `Tsk.Start` 및 `Tsk.Finish` 날짜는 상위 `Tsk.Start` 및 `Tsk.Finish` 날짜를 기준으로 ALAP로 일정이 잡히며 `Project.TaskLinks`를 고려합니다. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Task`의 `Tsk.Start` 및 `Tsk.Finish` 날짜는 상위 `Tsk.Start` 및 `Tsk.Finish` 날짜를 기준으로 ASAP으로 일정이 잡히며 `Project.TaskLinks`를 고려합니다. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | 완료 날짜는 이전에 있을 수 없습니다 |
| [FinishNoLaterThan](#FinishNoLaterThan) | 완료 날짜는 이후에 있을 수 없습니다 |
| [MustFinishOn](#MustFinishOn) | 완료 날짜는 반드시 이 날이어야 함 |
| [MustStartOn](#MustStartOn) | 시작 날짜는 반드시 이 날이어야 함 |
| [StartNoEarlierThan](#StartNoEarlierThan) | 시작 날짜는 이전에 있을 수 없습니다 |
| [StartNoLaterThan](#StartNoLaterThan) | 시작 날짜는 이후에 있을 수 없습니다 |
| [Undefined](#Undefined) | 원본 프로젝트 파일에 값이 정의되지 않았습니다. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Task`의 `Tsk.Start` 및 `Tsk.Finish` 날짜는 상위 `Tsk.Start` 및 `Tsk.Finish` 날짜를 기준으로 ALAP로 일정이 잡히며 `Project.TaskLinks`를 고려합니다.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Task`의 `Tsk.Start` 및 `Tsk.Finish` 날짜는 상위 `Tsk.Start` 및 `Tsk.Finish` 날짜를 기준으로 ASAP으로 일정이 잡히며 `Project.TaskLinks`를 고려합니다.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


완료 날짜는 이전에 있을 수 없습니다

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


완료 날짜는 이후에 있을 수 없습니다

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


완료 날짜는 반드시 이 날이어야 함

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


시작 날짜는 반드시 이 날이어야 함

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


시작 날짜는 이전에 있을 수 없습니다

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


시작 날짜는 이후에 있을 수 없습니다

### Undefined {#Undefined}
```
public static final int Undefined
```


원본 프로젝트 파일에 값이 정의되지 않았습니다.

