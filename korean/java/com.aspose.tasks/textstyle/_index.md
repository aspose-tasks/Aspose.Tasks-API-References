---
title: "TextStyle"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 보기에서 항목의 텍스트 시각적 스타일을 변경합니다."
type: docs
weight: 315
url: /ko/java/com.aspose.tasks/textstyle/
---

**Inheritance:**
java.lang.Object
```
public class TextStyle
```

프로젝트 보기에서 항목의 텍스트 시각적 스타일을 변경합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TextStyle()](#TextStyle--) | 기본 설정으로 [TextStyle](../../com.aspose.tasks/textstyle) 클래스를 새 인스턴스로 초기화합니다. |
| [TextStyle(float fontSize, int fontStyle)](#TextStyle-float-int-) | 기본 글꼴과 지정된 글꼴 크기 및 스타일을 사용하여 [TextStyle](../../com.aspose.tasks/textstyle) 클래스를 새 인스턴스로 초기화합니다. |
| [TextStyle(int fontStyle)](#TextStyle-int-) | 기본 글꼴과 지정된 글꼴 스타일을 사용하여 [TextStyle](../../com.aspose.tasks/textstyle) 클래스를 새 인스턴스로 초기화합니다. |
| [TextStyle(FontDescriptor font)](#TextStyle-com.aspose.tasks.FontDescriptor-) | 지정된 글꼴 설정으로 [TextStyle](../../com.aspose.tasks/textstyle) 클래스를 새 인스턴스로 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--) | 텍스트 스타일의 배경 색상을 가져옵니다. |
| [getBackgroundPattern()](#getBackgroundPattern--) | 텍스트 스타일의 배경 패턴을 가져옵니다. |
| [getColor()](#getColor--) | 텍스트의 색상을 가져옵니다. |
| [getFont()](#getFont--) | 텍스트 스타일의 글꼴을 가져옵니다. |
| [getItemType()](#getItemType--) | 텍스트 스타일의 [TextItemType](../../com.aspose.tasks/textitemtype)을 가져옵니다. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | 텍스트 스타일의 배경 색상을 설정합니다. |
| [setBackgroundPattern(int value)](#setBackgroundPattern-int-) | 텍스트 스타일의 배경 패턴을 설정합니다. |
| [setColor(Color value)](#setColor-java.awt.Color-) | 텍스트의 색상을 설정합니다. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | 텍스트 스타일의 글꼴을 설정합니다. |
| [setItemType(int value)](#setItemType-int-) | 텍스트 스타일의 [TextItemType](../../com.aspose.tasks/textitemtype)을 설정합니다. |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


기본 설정으로 [TextStyle](../../com.aspose.tasks/textstyle) 클래스를 새 인스턴스로 초기화합니다.

### TextStyle(float fontSize, int fontStyle) {#TextStyle-float-int-}
```
public TextStyle(float fontSize, int fontStyle)
```


기본 글꼴과 지정된 글꼴 크기 및 스타일을 사용하여 [TextStyle](../../com.aspose.tasks/textstyle) 클래스를 새 인스턴스로 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fontSize | float | TextStyle의 글꼴 크기. |
| fontStyle | int | TextStyle의 글꼴 스타일. |

### TextStyle(int fontStyle) {#TextStyle-int-}
```
public TextStyle(int fontStyle)
```


기본 글꼴과 지정된 글꼴 스타일을 사용하여 [TextStyle](../../com.aspose.tasks/textstyle) 클래스를 새 인스턴스로 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fontStyle | int | 기본 글꼴에 적용할 글꼴 스타일. |

### TextStyle(FontDescriptor font) {#TextStyle-com.aspose.tasks.FontDescriptor-}
```
public TextStyle(FontDescriptor font)
```


지정된 글꼴 설정으로 [TextStyle](../../com.aspose.tasks/textstyle) 클래스를 새 인스턴스로 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | TextStyle의 글꼴. |

### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


텍스트 스타일의 배경 색상을 가져옵니다. `Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Returns:**
java.awt.Color - 텍스트 스타일의 배경 색상.
### getBackgroundPattern() {#getBackgroundPattern--}
```
public final int getBackgroundPattern()
```


텍스트 스타일의 배경 패턴을 가져옵니다. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Returns:**
int - 텍스트 스타일의 배경 패턴.
### getColor() {#getColor--}
```
public final Color getColor()
```


텍스트의 색상을 가져옵니다.

**Returns:**
java.awt.Color - 텍스트 색상.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


텍스트 스타일의 글꼴을 가져옵니다.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - font of the text style.
### getItemType() {#getItemType--}
```
public int getItemType()
```


텍스트 스타일의 [TextItemType](../../com.aspose.tasks/textitemtype)을 가져옵니다.

**Returns:**
int - 텍스트 스타일의 [TextItemType](../../com.aspose/tasks/textitemtype).
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


텍스트 스타일의 배경 색상을 설정합니다. `Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 텍스트 스타일의 배경 색상. |

### setBackgroundPattern(int value) {#setBackgroundPattern-int-}
```
public final void setBackgroundPattern(int value)
```


텍스트 스타일의 배경 패턴을 설정합니다. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 텍스트 스타일의 배경 패턴. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public final void setColor(Color value)
```


텍스트의 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 텍스트 색상. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


텍스트 스타일의 글꼴을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 텍스트 스타일의 글꼴. |

### setItemType(int value) {#setItemType-int-}
```
public void setItemType(int value)
```


텍스트 스타일의 [TextItemType](../../com.aspose.tasks/textitemtype)을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | 텍스트 스타일의 [TextItemType](../../com.aspose.tasks/textitemtype). |

