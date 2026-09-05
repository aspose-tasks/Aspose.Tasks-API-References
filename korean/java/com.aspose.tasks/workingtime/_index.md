---
title: "WorkingTime"
second_title: "Aspose.Tasks for Java API Reference"
description: "평일 동안의 작업 시간을 나타냅니다."
type: docs
weight: 365
url: /ko/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

평일 동안의 작업 시간을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | 지정된 시작 및 종료 시간으로 구간을 사용하여 [WorkingTime](../../com.aspose.tasks/workingtime) 클래스의 새 인스턴스를 초기화합니다. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | 지정된 시작 및 종료 시간으로 구간 항목을 사용하여 [WorkingTime](../../com.aspose.tasks/workingtime) 클래스의 새 인스턴스를 초기화합니다. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | 지정된 시작 및 종료 시간으로 구간 항목을 사용하여 [WorkingTime](../../com.aspose.tasks/workingtime) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | 객체가 동일한지 확인합니다. |
| [getFrom()](#getFrom--) | 작업 시간의 시작을 가져옵니다. |
| [getTo()](#getTo--) | 작업 시간의 끝을 가져옵니다. |
| [hashCode()](#hashCode--) | [WorkingTime](../../com.aspose.tasks/workingtime) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


지정된 시작 및 종료 시간으로 구간을 사용하여 [WorkingTime](../../com.aspose.tasks/workingtime) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fromTime | java.util.Date | 구간 시작 시간 |
| toTime | java.util.Date | 구간 종료 시간 |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


지정된 시작 및 종료 시간으로 구간 항목을 사용하여 [WorkingTime](../../com.aspose.tasks/workingtime) 클래스의 새 인스턴스를 초기화합니다.

--------------------

&gt; ```
&gt; WorkingTime 생성자의 오버로드를 사용하여 TimeSpan을 이용해 구간의 시작과 끝을 초기화할 수 있습니다:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fromHours | int | 구간 시작 시간은 전체 시간(0-24)으로 표시됩니다. |
| toHours | int | 구간 종료 시간은 전체 시간(0-24)으로 표시됩니다. |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


객체가 동일한지 확인합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 비교할 두 번째 객체. |

**Returns:**
boolean - 객체가 동일하면 true, 그렇지 않으면 false.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


작업 시간의 시작을 가져옵니다.

**Returns:**
java.util.Date - 작업 시간의 시작.
### getTo() {#getTo--}
```
public final Date getTo()
```


작업 시간의 끝을 가져옵니다.

**Returns:**
java.util.Date - 작업 시간의 끝.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[WorkingTime](../../com.aspose.tasks/workingtime) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
