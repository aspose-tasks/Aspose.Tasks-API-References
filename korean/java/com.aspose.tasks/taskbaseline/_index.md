---
title: "TaskBaseline"
second_title: "Aspose.Tasks for Java API Reference"
description: "작업의 기준선을 나타냅니다."
type: docs
weight: 291
url: /ko/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

작업의 기준선을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | 새로운 [TaskBaseline](../../com.aspose.tasks/taskbaseline) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | IComparable 인터페이스 구현. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | 이 인스턴스가 지정된 TaskBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getDuration()](#getDuration--) | 베이스라인이 저장될 때 작업의 예정 지속 시간을 가져옵니다. |
| [getEstimatedDuration()](#getEstimatedDuration--) | 작업의 베이스라인 지속 시간이 추정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getFinish()](#getFinish--) | 베이스라인이 저장될 때 작업의 예정 종료 날짜를 가져옵니다. |
| [getFixedCost()](#getFixedCost--) | 베이스라인이 저장될 때 작업의 고정 비용을 가져옵니다. |
| [getInterim()](#getInterim--) | 이것이 중간 베이스라인인지 여부를 나타내는 값을 가져옵니다. |
| [getStart()](#getStart--) | 베이스라인이 저장될 때 작업의 예정 시작 날짜를 가져옵니다. |
| [getTimephasedData()](#getTimephasedData--) | 이 객체에 대한 TimephasedDataCollection 인스턴스를 가져옵니다. |
| [hashCode()](#hashCode--) | [TaskBaseline](../../com.aspose.tasks/taskbaseline) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | 베이스라인이 저장될 때 작업의 예정 지속 시간을 설정합니다. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | 작업의 베이스라인 지속 시간이 추정되었는지 여부를 나타내는 값을 설정합니다. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 베이스라인이 저장될 때 작업의 예정 종료 날짜를 설정합니다. |
| [setFixedCost(double value)](#setFixedCost-double-) | 베이스라인이 저장될 때 작업의 고정 비용을 설정합니다. |
| [setInterim(boolean value)](#setInterim-boolean-) | 이것이 중간 베이스라인인지 여부를 나타내는 값을 설정합니다. |
| [setStart(Date value)](#setStart-java.util.Date-) | 베이스라인이 저장될 때 작업의 예정 시작 날짜를 설정합니다. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | 이 객체에 대한 TimephasedDataCollection 인스턴스를 설정합니다. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


새로운 [TaskBaseline](../../com.aspose.tasks/taskbaseline) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 베이스라인의 상위 작업. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


IComparable 인터페이스 구현. 이 인스턴스를 지정된 Baseline 객체와 비교합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | 이 인스턴스를 비교할 지정된 Baseline 객체. |

**Returns:**
int - 이 인스턴스가 지정된 객체보다 작으면 -1을 반환하고, 크면 1을 반환합니다; 그 외의 경우 0을 반환합니다.
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


이 인스턴스가 지정된 TaskBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | 이 인스턴스와 비교할 지정된 AssignmentBaseline 객체. |

**Returns:**
boolean - 이 인스턴스가 지정된 TaskBaseline 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 객체입니다. |

**Returns:**
boolean - 지정된 객체가 이 인스턴스와 동일한 UID 값을 가진 TaskBaseline인 경우 **True**, 그렇지 않으면 **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


베이스라인이 저장될 때 작업의 예정 지속 시간을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


작업의 베이스라인 지속 시간이 추정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 작업의 베이스라인 지속 시간이 추정되었는지 여부를 나타내는 값.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


베이스라인이 저장될 때 작업의 예정 종료 날짜를 가져옵니다.

**Returns:**
java.util.Date - 베이스라인이 저장될 때 작업의 예정 종료 날짜.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


베이스라인이 저장될 때 작업의 고정 비용을 가져옵니다.

**Returns:**
double - 기준선이 저장될 때 작업의 고정 비용.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


이것이 중간 베이스라인인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 이것이 중간 기준선인지 여부를 나타내는 값.
### getStart() {#getStart--}
```
public final Date getStart()
```


베이스라인이 저장될 때 작업의 예정 시작 날짜를 가져옵니다.

**Returns:**
java.util.Date - 기준선이 저장될 때 작업의 예정 시작 날짜.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


이 객체에 대한 TimephasedDataCollection 인스턴스를 가져옵니다. 작업 기준선과 연결된 시간 구분 데이터.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[TaskBaseline](../../com.aspose.tasks/taskbaseline) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


베이스라인이 저장될 때 작업의 예정 지속 시간을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 기준선이 저장될 때 작업의 예정 지속 시간. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


작업의 베이스라인 지속 시간이 추정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 작업의 기준선 지속 시간이 추정되었는지 여부를 나타내는 값. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


베이스라인이 저장될 때 작업의 예정 종료 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 기준선이 저장될 때 작업의 예정 완료 날짜. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


베이스라인이 저장될 때 작업의 고정 비용을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 기준선이 저장될 때 작업의 고정 비용. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


이것이 중간 베이스라인인지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 이것이 중간 기준선인지 여부를 나타내는 값. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


베이스라인이 저장될 때 작업의 예정 시작 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 기준선이 저장될 때 작업의 예정 시작 날짜. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


이 객체에 대한 TimephasedDataCollection 인스턴스를 설정합니다. 작업 기준선과 연결된 시간 구분 데이터.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | 이 객체에 대한 TimephasedDataCollection 인스턴스. |

