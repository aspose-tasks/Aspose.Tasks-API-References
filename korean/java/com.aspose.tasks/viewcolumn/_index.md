---
title: "ViewColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 보기의 열을 나타냅니다."
type: docs
weight: 344
url: /ko/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

프로젝트 보기의 열을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getField()](#getField--) | 열 필드를 가져옵니다. |
| [getName()](#getName--) | 열 이름을 가져옵니다. |
| [getStringAlignment()](#getStringAlignment--) | 텍스트 정렬을 가져옵니다( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 열거형의 값 중 하나일 수 있습니다). |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | 열 셀의 모양을 사용자 정의하는 데 사용할 수 있는 콜백을 가져옵니다. |
| [getWidth()](#getWidth--) | 열 너비를 가져옵니다. |
| [setField(int value)](#setField-int-) | 열 필드를 설정합니다. |
| [setStringAlignment(int value)](#setStringAlignment-int-) | 텍스트 정렬을 설정합니다( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 열거형의 값 중 하나일 수 있습니다). |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | 열 셀의 모양을 사용자 정의하는 데 사용할 수 있는 콜백을 설정합니다. |
### getField() {#getField--}
```
public abstract int getField()
```


열 필드를 가져옵니다. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - 열 필드.
### getName() {#getName--}
```
public final String getName()
```


열 이름을 가져옵니다.

**Returns:**
java.lang.String - 열 이름.
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


텍스트 정렬을 가져옵니다( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 열거형의 값 중 하나일 수 있습니다).

**Returns:**
int - 텍스트 정렬( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 열거형의 값 중 하나일 수 있습니다).
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


열 셀의 모양을 사용자 정의하는 데 사용할 수 있는 콜백을 가져옵니다.

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


열 너비를 가져옵니다.

**Returns:**
int - 열 너비.
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


열 필드를 설정합니다. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 열 필드. |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


텍스트 정렬을 설정합니다( [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) 열거형의 값 중 하나일 수 있습니다).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | 텍스트 정렬 (다음 [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) 열거형 값 중 하나일 수 있음). |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


열 셀의 모양을 사용자 정의하는 데 사용할 수 있는 콜백을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | 열의 셀 모양을 사용자 정의하는 데 사용할 수 있는 콜백. |

