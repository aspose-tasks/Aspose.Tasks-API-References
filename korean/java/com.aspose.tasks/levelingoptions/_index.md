---
title: "LevelingOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "리소스 레벨링 매개변수를 지정할 수 있습니다."
type: docs
weight: 142
url: /ko/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

리소스 레벨링 매개변수를 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | 새 인스턴스를 초기화합니다 [LevelingOptions](../../com.aspose.tasks/levelingoptions) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | 프로젝트 레벨링 작업을 취소하는 데 사용할 수 있는 토큰을 가져옵니다. |
| [getFinishDate()](#getFinishDate--) | 레벨링 기간 종료 날짜를 가져옵니다. |
| [getLevelingOrder()](#getLevelingOrder--) | 레벨링 알고리즘이 과다 할당된 작업을 지연시키는 순서를 가져옵니다. |
| [getMessageHandler()](#getMessageHandler--) | 리소스 레벨링 중 Aspose.Tasks에서 생성된 로그 메시지를 가로챌 수 있는 메시지 핸들러 콜백을 가져옵니다. |
| [getMessageLevel()](#getMessageLevel--) | 리소스 레벨링 중 Aspose.Tasks에서 발생하는 로그 메시지 수준을 가져옵니다. |
| [getResources()](#getResources--) | 레벨링될 리소스 목록을 가져옵니다. |
| [getStartDate()](#getStartDate--) | 레벨링 기간 시작 날짜를 가져옵니다. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | 프로젝트 레벨링 작업을 취소하는 데 사용할 수 있는 토큰을 설정합니다. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | 레벨링 기간 종료 날짜를 설정합니다. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | 레벨링 알고리즘이 과다 할당된 작업을 지연시키는 순서. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | 리소스 레벨링 중 Aspose.Tasks에서 생성된 로그 메시지를 가로챌 수 있는 메시지 핸들러 콜백을 설정합니다. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | 리소스 레벨링 중 Aspose.Tasks에서 발생하는 로그 메시지 수준을 설정합니다. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | 레벨링될 리소스 목록을 설정합니다. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | 레벨링 기간 시작 날짜를 설정합니다. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


새 인스턴스를 초기화합니다 [LevelingOptions](../../com.aspose.tasks/levelingoptions) 클래스.

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


프로젝트 레벨링 작업을 취소하는 데 사용할 수 있는 토큰을 가져옵니다.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


레벨링 기간 종료 날짜를 가져옵니다. 기본값은 프로젝트의 종료 날짜입니다.

**Returns:**
java.util.Date - 레벨링 기간 종료 날짜.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


레벨링 알고리즘이 과다 할당된 작업을 지연시키는 순서를 가져옵니다. 과다 할당을 일으키는 작업과 지연시킬 수 있는 작업을 결정한 후, 지정된 순서에 따라 먼저 지연시킬 작업이 선택됩니다.

**Returns:**
int - 레벨링 알고리즘이 과다 할당된 작업을 지연시키는 순서.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


리소스 레벨링 중 Aspose.Tasks에서 생성된 로그 메시지를 가로챌 수 있는 메시지 핸들러 콜백을 가져옵니다.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


리소스 레벨링 중 Aspose.Tasks에서 발생하는 로그 메시지 수준을 가져옵니다.

**Returns:**
int - Aspose에서 발생하는 로그 메시지의 수준.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


레벨링될 리소스 목록을 가져옵니다. null이 설정된 경우, 모든 프로젝트 리소스가 레벨링됩니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - 레벨링될 리소스 목록.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


레벨링 기간 시작 날짜를 가져옵니다. 기본값은 프로젝트의 시작 날짜입니다.

**Returns:**
java.util.Date - 레벨링 기간 시작 날짜.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


프로젝트 레벨링 작업을 취소하는 데 사용할 수 있는 토큰을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | 프로젝트 레벨링 작업을 취소하는 데 사용할 수 있는 토큰. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


레벨링 기간 종료 날짜를 설정합니다. 기본값은 프로젝트의 종료 날짜입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 레벨링 기간 종료 날짜. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


레벨링 알고리즘이 과다 할당된 작업을 지연시키는 순서입니다. 과다 할당을 일으키는 작업과 지연시킬 수 있는 작업을 결정한 후, 지정된 순서에 따라 먼저 지연시킬 작업이 선택됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 레벨링 알고리즘이 과다 할당된 작업을 지연시키는 순서. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


리소스 레벨링 중 Aspose.Tasks에서 생성된 로그 메시지를 가로챌 수 있는 메시지 핸들러 콜백을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | Aspose에서 생성된 로그 메시지를 가로챌 수 있는 메시지 핸들러 콜백. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


리소스 레벨링 중 Aspose.Tasks에서 발생하는 로그 메시지 수준을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Aspose에서 발생하는 로그 메시지의 수준. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


레벨링될 리소스 목록을 설정합니다. null이 설정된 경우, 모든 프로젝트 리소스가 레벨링됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.List&lt;com.aspose.tasks.Resource&gt; | 레벨링될 리소스 목록. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


레벨링 기간 시작 날짜를 설정합니다. 기본값은 프로젝트의 시작 날짜입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 레벨링 기간 시작 날짜. |

