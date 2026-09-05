---
title: "AssignmentBaseline"
second_title: "Aspose.Tasks for Java API Reference"
description: "리소스 할당의 기준선을 나타냅니다."
type: docs
weight: 17
url: /ko/java/com.aspose.tasks/assignmentbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)
```
public class AssignmentBaseline extends Baseline
```

리소스 할당의 기준선을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AssignmentBaseline()](#AssignmentBaseline--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [compareTo(AssignmentBaseline other)](#compareTo-com.aspose.tasks.AssignmentBaseline-) | IComparable 인터페이스 구현. |
| [equals(AssignmentBaseline other)](#equals-com.aspose.tasks.AssignmentBaseline-) | 이 인스턴스가 지정된 AssignmentBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getFinish()](#getFinish--) | 베이스라인이 저장될 때 리소스 할당의 예정 완료 날짜를 가져옵니다. |
| [getStart()](#getStart--) | 베이스라인이 저장될 때 리소스 할당의 예정 시작 날짜를 가져옵니다. |
| [getTimephasedData()](#getTimephasedData--) | 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 인스턴스를 가져옵니다. |
| [hashCode()](#hashCode--) | 이 AssignmentBaseline에 대한 해시 코드 값을 반환합니다. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | 베이스라인이 저장될 때 리소스 할당의 예정 완료 날짜를 설정합니다. |
| [setStart(Date value)](#setStart-java.util.Date-) | 베이스라인이 저장될 때 리소스 할당의 예정 시작 날짜를 설정합니다. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 인스턴스를 설정합니다. |
### AssignmentBaseline() {#AssignmentBaseline--}
```
public AssignmentBaseline()
```


### compareTo(AssignmentBaseline other) {#compareTo-com.aspose.tasks.AssignmentBaseline-}
```
public final int compareTo(AssignmentBaseline other)
```


IComparable 인터페이스 구현. 이 인스턴스를 지정된 Baseline 객체와 비교합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | 이 인스턴스를 비교할 지정된 Baseline 객체. |

**Returns:**
int - 이 인스턴스가 지정된 객체보다 작으면 -1을 반환하고, 크면 1을 반환합니다; 그 외의 경우 0을 반환합니다.
### equals(AssignmentBaseline other) {#equals-com.aspose.tasks.AssignmentBaseline-}
```
public final boolean equals(AssignmentBaseline other)
```


이 인스턴스가 지정된 AssignmentBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | 이 인스턴스와 비교할 지정된 AssignmentBaseline 객체. |

**Returns:**
boolean - 이 인스턴스가 지정된 AssignmentBaseline 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 지정된 객체. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


베이스라인이 저장될 때 리소스 할당의 예정 완료 날짜를 가져옵니다.

값: 이 기준선이 저장될 때 리소스 할당의 종료 날짜.

**Returns:**
java.util.Date - 기준선이 저장될 때 리소스 할당의 예정 종료 날짜.
### getStart() {#getStart--}
```
public final Date getStart()
```


베이스라인이 저장될 때 리소스 할당의 예정 시작 날짜를 가져옵니다.

값: 이 기준선이 저장될 때 리소스 할당의 시작 날짜.

**Returns:**
java.util.Date - 기준선이 저장될 때 리소스 할당의 예정 시작 날짜.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 인스턴스를 가져옵니다. 리소스 할당 기준선과 연결된 시계열 데이터입니다.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) instance for this object. Value: The collection of Time phased data associated with this baseline.
### hashCode() {#hashCode--}
```
public int hashCode()
```


이 AssignmentBaseline에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


베이스라인이 저장될 때 리소스 할당의 예정 완료 날짜를 설정합니다.

값: 이 기준선이 저장될 때 리소스 할당의 종료 날짜.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 기준선이 저장될 때 리소스 할당의 예정 종료 날짜. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


베이스라인이 저장될 때 리소스 할당의 예정 시작 날짜를 설정합니다.

값: 이 기준선이 저장될 때 리소스 할당의 시작 날짜.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 기준선이 저장될 때 리소스 할당의 예정 시작 날짜. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 인스턴스를 설정합니다. 리소스 할당 기준선과 연결된 시계열 데이터입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | 이 객체에 대한 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 인스턴스. |

