---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트를 Project Server 또는 Project Online에 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 227
url: /ko/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

프로젝트를 Project Server 또는 Project Online에 저장할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | 새 인스턴스를 초기화합니다. [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | 큐 작업 상태 요청 간의 간격을 가져옵니다. |
| [getProjectGuid()](#getProjectGuid--) | 프로젝트의 고유 식별자를 가져옵니다. |
| [getProjectName()](#getProjectName--) | Project Server \\ Project Online 프로젝트 목록에 표시되는 프로젝트 이름을 가져옵니다. |
| [getTimeout()](#getTimeout--) | Project Server의 큐 처리 서비스가 저장 프로젝트 요청을 처리할 때 대기하는 데 사용되는 제한 시간을 가져옵니다. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | 큐 작업 상태 요청 간의 간격을 설정합니다. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | 프로젝트의 고유 식별자를 설정합니다. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Project Server \\ Project Online 프로젝트 목록에 표시되는 프로젝트 이름을 설정합니다. |
| [setTimeout(double value)](#setTimeout-double-) | Project Server의 큐 처리 서비스가 저장 프로젝트 요청을 처리할 때 대기하는 데 사용되는 제한 시간을 설정합니다. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


새 인스턴스를 초기화합니다. [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) 클래스.

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


큐 작업 상태 요청 간의 간격을 가져옵니다. 기본값은 2초입니다.

**Returns:**
double - 큐 작업 상태 요청 간의 간격.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


프로젝트의 고유 식별자를 가져옵니다. Project Server \\ Project Online 인스턴스 내에서 고유해야 합니다.

**Returns:**
java.util.UUID - 프로젝트의 고유 식별자.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Project Server \\ Project Online 프로젝트 목록에 표시되는 프로젝트 이름을 가져옵니다. Project Server \\ Project Online 인스턴스 내에서 고유해야 합니다. 값이 생략되면 Prj.Name 속성의 값이 대신 사용됩니다.

**Returns:**
java.lang.String - Project Server \\ Project Online 프로젝트 목록에 표시되는 프로젝트 이름.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Project Server의 큐 처리 서비스가 저장 프로젝트 요청을 처리할 때 대기하는 데 사용되는 제한 시간을 가져옵니다. 이 속성의 기본값은 1분입니다.

--------------------

대규모 프로젝트의 경우 또는 Project Server 인스턴스가 다른 요청에 응답하느라 너무 바쁠 경우 처리 시간이 더 길어질 수 있습니다.

**Returns:**
double - Project Server의 큐 처리 서비스가 저장 프로젝트 요청을 처리할 때 대기하는 데 사용되는 제한 시간.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


큐 작업 상태 요청 간의 간격을 설정합니다. 기본값은 2초입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 큐 작업 상태 요청 간의 간격. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


프로젝트의 고유 식별자를 설정합니다. Project Server \\ Project Online 인스턴스 내에서 고유해야 합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.UUID | 프로젝트의 고유 식별자. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Project Server \\ Project Online 프로젝트 목록에 표시되는 프로젝트 이름을 설정합니다. Project Server \\ Project Online 인스턴스 내에서 고유해야 합니다. 값이 생략되면 Prj.Name 속성의 값이 대신 사용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Project Server \\ Project Online 프로젝트 목록에 표시되는 프로젝트 이름. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Project Server의 큐 처리 서비스가 저장 프로젝트 요청을 처리할 때 대기하는 데 사용되는 제한 시간을 설정합니다. 이 속성의 기본값은 1분입니다.

--------------------

대규모 프로젝트의 경우 또는 Project Server 인스턴스가 다른 요청에 응답하느라 너무 바쁠 경우 처리 시간이 더 길어질 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | 프로젝트 서버의 대기열 처리 서비스가 저장 프로젝트 요청을 처리할 때 대기하는 데 사용되는 시간 초과. |

