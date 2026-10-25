---
title: "GroupCriterion"
second_title: "Aspose.Tasks for Java API Reference"
description: "그룹 정의의 기준을 나타냅니다."
type: docs
weight: 124
url: /ko/java/com.aspose.tasks/groupcriterion/
---

**Inheritance:**
java.lang.Object
```
public class GroupCriterion
```

그룹 정의에서 기준을 나타냅니다. GroupCriterion 객체는 [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection) 컬렉션의 구성원입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GroupCriterion()](#GroupCriterion--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getAscending()](#getAscending--) | 그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값을 가져옵니다. |
| [getCellColor()](#getCellColor--) | 그룹 정의에서 기준으로 사용되는 필드의 셀 배경 색상을 가져옵니다. |
| [getField()](#getField--) | 그룹화되는 필드를 가져옵니다. |
| [getFont()](#getFont--) | 그룹 정의에서 기준의 글꼴을 가져옵니다. |
| [getFontColor()](#getFontColor--) | 그룹 정의에서 기준으로 사용되는 필드의 글꼴 색상을 가져옵니다. |
| [getGroupInterval()](#getGroupInterval--) | 그룹 정의에서 기준으로 사용되는 필드의 간격을 가져옵니다. |
| [getGroupOn()](#getGroupOn--) | 그룹 정의에서 기준으로 사용되는 필드의 그룹화 유형을 가져옵니다. |
| [getPattern()](#getPattern--) | 그룹 정의에서 기준으로 사용되는 필드의 셀 패턴을 가져옵니다. |
| [getStartAt()](#getStartAt--) | 그룹 정의에서 기준으로 사용되는 필드의 간격 시작값을 가져옵니다. |
| [hashCode()](#hashCode--) | 특정 유형에 대한 해시 함수 역할을 합니다. |
| [setAscending(boolean value)](#setAscending-boolean-) | 그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값을 설정합니다. |
| [setCellColor(Color value)](#setCellColor-java.awt.Color-) | 그룹 정의에서 기준으로 사용되는 필드의 셀 배경 색상을 설정합니다. |
| [setField(int value)](#setField-int-) | 그룹화되는 필드를 설정합니다. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | 그룹 정의에서 기준의 글꼴을 설정합니다. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | 그룹 정의에서 기준으로 사용되는 필드의 글꼴 색상을 설정합니다. |
| [setGroupInterval(Object value)](#setGroupInterval-java.lang.Object-) | 그룹 정의에서 기준으로 사용되는 필드의 간격을 설정합니다. |
| [setGroupOn(int value)](#setGroupOn-int-) | 그룹 정의에서 기준으로 사용되는 필드의 그룹화 유형을 설정합니다. |
| [setPattern(int value)](#setPattern-int-) | 그룹 정의에서 기준으로 사용되는 필드의 셀 패턴을 설정합니다. |
| [setStartAt(Object value)](#setStartAt-java.lang.Object-) | 그룹 정의에서 기준으로 사용되는 필드의 구간 시작을 설정합니다. |
### GroupCriterion() {#GroupCriterion--}
```
public GroupCriterion()
```


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
boolean - **True**이면 o가 이 인스턴스와 동일한 UID 값을 가진 GroupCriterion이며, 그렇지 않으면 **false**.
### getAscending() {#getAscending--}
```
public final boolean getAscending()
```


그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값을 가져옵니다. 필드가 내림차순으로 정렬된 경우 False.

**Returns:**
boolean - 그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값.
### getCellColor() {#getCellColor--}
```
public final Color getCellColor()
```


그룹 정의에서 기준으로 사용되는 필드의 셀 배경 색상을 가져옵니다.

**Returns:**
java.awt.Color - 그룹 정의에서 기준으로 사용되는 필드의 셀 배경 색상.
### getField() {#getField--}
```
public final int getField()
```


그룹화되는 필드를 가져옵니다.

**Returns:**
int - 그룹화되는 필드.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


그룹 정의에서 기준의 글꼴을 가져옵니다.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font for a criterion in a group definition.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


그룹 정의에서 기준으로 사용되는 필드의 글꼴 색상을 가져옵니다.

**Returns:**
java.awt.Color - 그룹 정의에서 기준으로 사용되는 필드의 글꼴 색상.
### getGroupInterval() {#getGroupInterval--}
```
public final Object getGroupInterval()
```


그룹 정의에서 기준으로 사용되는 필드의 간격을 가져옵니다.

**Returns:**
java.lang.Object - 그룹 정의에서 기준으로 사용되는 필드의 구간.
### getGroupOn() {#getGroupOn--}
```
public final int getGroupOn()
```


그룹 정의에서 기준으로 사용되는 필드의 그룹화 유형을 가져옵니다.

**Returns:**
int - 그룹 정의에서 기준으로 사용되는 필드의 그룹화 유형.
### getPattern() {#getPattern--}
```
public final int getPattern()
```


그룹 정의에서 기준으로 사용되는 필드의 셀 패턴을 가져옵니다.

**Returns:**
int - 그룹 정의에서 기준으로 사용되는 필드의 셀 패턴.
### getStartAt() {#getStartAt--}
```
public final Object getStartAt()
```


그룹 정의에서 기준으로 사용되는 필드의 간격 시작값을 가져옵니다.

**Returns:**
java.lang.Object - 그룹 정의에서 기준으로 사용되는 필드의 구간 시작.
### hashCode() {#hashCode--}
```
public int hashCode()
```


특정 유형에 대한 해시 함수 역할을 합니다.

**Returns:**
int - 현재 Object의 해시 코드.
### setAscending(boolean value) {#setAscending-boolean-}
```
public final void setAscending(boolean value)
```


그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값을 설정합니다. 필드가 내림차순으로 정렬된 경우 False.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값. |

### setCellColor(Color value) {#setCellColor-java.awt.Color-}
```
public final void setCellColor(Color value)
```


그룹 정의에서 기준으로 사용되는 필드의 셀 배경 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 그룹 정의에서 기준으로 사용되는 필드의 셀 배경 색상. |

### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


그룹화되는 필드를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 그룹화되는 필드. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


그룹 정의에서 기준의 글꼴을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 그룹 정의에서 기준의 글꼴. |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


그룹 정의에서 기준으로 사용되는 필드의 글꼴 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 그룹 정의에서 기준으로 사용되는 필드의 글꼴 색상. |

### setGroupInterval(Object value) {#setGroupInterval-java.lang.Object-}
```
public final void setGroupInterval(Object value)
```


그룹 정의에서 기준으로 사용되는 필드의 간격을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Object | 그룹 정의에서 기준으로 사용되는 필드의 구간. |

### setGroupOn(int value) {#setGroupOn-int-}
```
public final void setGroupOn(int value)
```


그룹 정의에서 기준으로 사용되는 필드의 그룹화 유형을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 그룹 정의에서 기준으로 사용되는 필드의 그룹화 유형. |

### setPattern(int value) {#setPattern-int-}
```
public final void setPattern(int value)
```


그룹 정의에서 기준으로 사용되는 필드의 셀 패턴을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 그룹 정의에서 기준으로 사용되는 필드의 셀 패턴. |

### setStartAt(Object value) {#setStartAt-java.lang.Object-}
```
public final void setStartAt(Object value)
```


그룹 정의에서 기준으로 사용되는 필드의 구간 시작을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Object | 그룹 정의에서 기준으로 사용되는 필드의 구간 시작. |

