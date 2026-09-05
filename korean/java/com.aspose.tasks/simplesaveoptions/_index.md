---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "특정 형식으로 프로젝트를 저장할 때 사용자가 기본 옵션을 지정할 수 있도록 하는 추상 기본 클래스입니다."
type: docs
weight: 277
url: /ko/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

특정 형식으로 프로젝트를 저장할 때 사용자가 기본 옵션을 지정할 수 있도록 하는 추상 기본 클래스입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | 이 저장 옵션 객체가 사용될 경우 문서가 저장될 형식을 가져옵니다. |
| [getTasksComparer()](#getTasksComparer--) | Gantt 차트와 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져옵니다. |
| [getTasksFilter()](#getTasksFilter--) | Gantt, 작업 시트 및 작업 사용 차트에 표시되는 작업을 필터링하는 데 사용되는 조건을 가져옵니다. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Gantt 차트와 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 설정합니다. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Gantt, 작업 시트 및 작업 사용 차트에 표시되는 작업을 필터링하는 데 사용되는 조건을 설정합니다. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


이 저장 옵션 객체가 사용될 경우 문서가 저장될 형식을 가져옵니다.

**Returns:**
int - 문서가 저장될 [SaveFileFormat](../../com.aspose.tasks/savefileformat)입니다.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Gantt 차트와 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져옵니다.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - Gantt 차트와 작업 시트 차트에서 작업을 정렬하기 위한 비교자.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Gantt, 작업 시트 및 작업 사용 차트에 표시되는 작업을 필터링하는 데 사용되는 조건을 가져옵니다.

--------------------

값이 지정되지 않으면 기본 필터가 사용되어 보이지 않는 작업(즉, 축소된 작업의 하위 작업)을 제거합니다.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Gantt 차트와 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | Gantt 차트와 작업 시트 차트에서 작업을 정렬하기 위한 비교자. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Gantt, 작업 시트 및 작업 사용 차트에 표시되는 작업을 필터링하는 데 사용되는 조건을 설정합니다.

--------------------

값이 지정되지 않으면 기본 필터가 사용되어 보이지 않는 작업(즉, 축소된 작업의 하위 작업)을 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Gantt, 작업 시트 및 작업 사용 차트에 표시되는 작업을 필터링하는 데 사용되는 조건. |

