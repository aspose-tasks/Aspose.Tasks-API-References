---
title: "OutlineValue"
second_title: "Aspose.Tasks for Java API Reference"
description: "개요 값을 나타냅니다."
type: docs
weight: 173
url: /ko/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

개요 값을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDescription()](#getDescription--) | 개요 값의 설명을 가져옵니다. |
| [getDurationValue()](#getDurationValue--) | Type이 Duration인 경우 지속 시간을 가져옵니다. |
| [getParentValueId()](#getParentValueId--) | 개요 코드의 상위 노드 ID를 가져옵니다. |
| [getType()](#getType--) | 개요 코드 유형을 가져옵니다. |
| [getValue()](#getValue--) | 실제 값을 가져옵니다. |
| [getValueGuid()](#getValueGuid--) | 전체 프로젝트에서 이 값을 다른 값과 구별하는 GUID를 가져옵니다. |
| [getValueId()](#getValueId--) | 프로젝트 내에서 개요 코드 값의 고유 Id를 가져옵니다. |
| [isCollapsed()](#isCollapsed--) | 개요 값이 축소되었는지 여부를 나타내는 값을 가져옵니다. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | 개요 값이 축소되었는지 여부를 나타내는 값을 설정합니다. |
| [setDescription(String value)](#setDescription-java.lang.String-) | 개요 값의 설명을 설정합니다. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Type이 Duration인 경우 기간을 설정합니다. |
| [setParentValueId(int value)](#setParentValueId-int-) | 개요 코드의 상위 노드 Id를 설정합니다. |
| [setType(int value)](#setType-int-) | 개요 코드 유형을 설정합니다. |
| [setValue(String value)](#setValue-java.lang.String-) | 실제 값을 설정합니다. |
| [setValueId(int value)](#setValueId-int-) | 프로젝트 내 개요 코드 값의 고유 Id를 설정합니다. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


개요 값의 설명을 가져옵니다.

**Returns:**
java.lang.String - 개요 값의 설명.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Type이 Duration인 경우 지속 시간을 가져옵니다.

--------------------

Duration 유형을 가진 OutlineValues의 값을 설정해야 할 때, `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-))보다 이 속성을 사용하십시오.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


개요 코드의 상위 노드 ID를 가져옵니다.

**Returns:**
int - 개요 코드의 상위 노드 Id.
### getType() {#getType--}
```
public final int getType()
```


개요 코드 유형을 가져옵니다.

**Returns:**
int - 개요 코드 유형.
### getValue() {#getValue--}
```
public final String getValue()
```


실제 값을 가져옵니다.

**Returns:**
java.lang.String - 실제 값.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


전체 프로젝트에서 이 값을 다른 값과 구별하는 GUID를 가져옵니다.

**Returns:**
java.util.UUID - 전체 프로젝트에서 이 값을 다른 값들과 구분하는 GUID입니다.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


프로젝트 내에서 개요 코드 값의 고유 Id를 가져옵니다.

**Returns:**
int - 프로젝트 내 개요 코드 값의 고유 Id.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


개요 값이 축소되었는지 여부를 나타내는 값을 가져옵니다.

--------------------

이 속성은 MS Project 2010에서 새롭게 추가되었습니다.

**Returns:**
boolean - 개요 값이 축소되었는지 여부를 나타내는 값.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


개요 값이 축소되었는지 여부를 나타내는 값을 설정합니다.

--------------------

이 속성은 MS Project 2010에서 새롭게 추가되었습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 개요 값이 축소되었는지 여부를 나타내는 값. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


개요 값의 설명을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 개요 값의 설명. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Type이 Duration인 경우 기간을 설정합니다.

--------------------

Duration 유형을 가진 OutlineValues의 값을 설정해야 할 때, `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-))보다 이 속성을 사용하십시오.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Type이 Duration인 경우 기간. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


개요 코드의 상위 노드 Id를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 개요 코드의 상위 노드 Id. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


개요 코드 유형을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 개요 코드 유형. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


실제 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 실제 값. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


프로젝트 내 개요 코드 값의 고유 Id를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 프로젝트 내 개요 코드 값의 고유 Id. |

