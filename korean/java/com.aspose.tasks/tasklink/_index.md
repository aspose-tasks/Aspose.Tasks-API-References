---
title: "TaskLink"
second_title: "Aspose.Tasks for Java API Reference"
description: "선행 작업 링크를 나타냅니다."
type: docs
weight: 295
url: /ko/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

선행 작업 링크를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getCrossProjectName()](#getCrossProjectName--) | 외부 선행 프로젝트를 가져옵니다. |
| [getLagFormat()](#getLagFormat--) | 지연 형식을 표현하는 포맷을 가져옵니다. |
| [getLinkLag()](#getLinkLag--) | 분의 10분의 1 또는 백분율 단위의 지연을 가져옵니다. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | LagFormat에 따라 지연 기간을 가져옵니다. |
| [getLinkType()](#getLinkType--) | 링크의 유형을 가져옵니다. |
| [getPredTask()](#getPredTask--) | 선행 작업을 가져옵니다. |
| [getSuccTask()](#getSuccTask--) | 후속 작업을 가져옵니다. |
| [hashCode()](#hashCode--) | 인스턴스인 [TaskLink](../../com.aspose.tasks/tasklink) 클래스에 대한 해시 코드 값을 반환합니다. |
| [isCrossProject()](#isCrossProject--) | 선행 작업이 다른 프로젝트의 일부인지 여부를 나타내는 값을 가져옵니다. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | 선행 작업이 다른 프로젝트의 일부인지 여부를 나타내는 값을 설정합니다. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | 외부 선행 프로젝트를 설정합니다. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | 지연 형식을 표현하는 형식을 설정합니다. |
| [setLinkLag(int value)](#setLinkLag-int-) | 분의 10분의 1 또는 백분율 단위로 지연을 설정합니다. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | LagFormat에 따라 지연 기간을 설정합니다. |
| [setLinkType(int value)](#setLinkType-int-) | 링크의 유형을 설정합니다. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | 선행 작업을 설정합니다. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | 후속 작업을 설정합니다. |
| [toString()](#toString--) | TaskLink의 문자열 표현을 반환합니다. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | 이 인스턴스와 비교할 지정된 [TaskLink](../../com.aspose.tasks/tasklink) 클래스의 인스턴스입니다. |

**Returns:**
boolean - 지정된 [TaskLink](../../com.aspose.tasks/tasklink) 클래스의 인스턴스가 이 인스턴스와 동일한 선행 및 후속 작업을 가지고 있는 경우 **True**; 그렇지 않으면 **false**.
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
boolean - 지정된 객체가 이 인스턴스와 동일한 선행 및 후속 작업을 가진 TaskLink인 경우 **True**; 그렇지 않으면 **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


외부 선행 프로젝트를 가져옵니다.

**Returns:**
java.lang.String - 외부 선행 프로젝트.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


지연 형식을 표현하는 포맷을 가져옵니다.

**Returns:**
byte - 지연 형식을 표현하는 형식.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


분의 10분의 1 또는 백분율 단위의 지연을 가져옵니다.

**Returns:**
int - 분의 10분의 1 또는 백분율 단위의 지연.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


LagFormat에 따라 지연 기간을 가져옵니다.

**Returns:**
double - LagFormat에 따라 지연 기간.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


링크의 유형을 가져옵니다.

**Returns:**
int - 링크의 유형.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


선행 작업을 가져옵니다.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


후속 작업을 가져옵니다.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


인스턴스인 [TaskLink](../../com.aspose.tasks/tasklink) 클래스에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


선행 작업이 다른 프로젝트의 일부인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 선행 작업이 다른 프로젝트의 일부인지 여부를 나타내는 값.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


선행 작업이 다른 프로젝트의 일부인지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 선행 작업이 다른 프로젝트의 일부인지 여부를 나타내는 값. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


외부 선행 프로젝트를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 외부 선행 프로젝트. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


지연 형식을 표현하는 형식을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | 바이트 | 지연 형식을 표현하는 형식. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


분의 10분의 1 또는 백분율 단위로 지연을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 분의 10분의 1 또는 백분율 단위의 지연. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


LagFormat에 따라 지연 기간을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | LagFormat에 따라 지연 기간. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


링크의 유형을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 링크 유형. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


선행 작업을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | 선행 작업. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


후속 작업을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | 후속 작업. |

### toString() {#toString--}
```
public String toString()
```


TaskLink의 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 명시되지 않았으며 변경될 수 있습니다.

**Returns:**
java.lang.String - TaskLink 객체를 나타내는 문자열.
