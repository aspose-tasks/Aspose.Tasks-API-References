---
title: "TableTextStyle"
second_title: "Aspose.Tasks for Java API Reference"
description: "뷰 테이블의 텍스트 스타일을 나타냅니다."
type: docs
weight: 288
url: /ko/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

뷰 테이블의 텍스트 스타일을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 클래스의 새 인스턴스를 초기화합니다. |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | 지정된 글꼴을 사용하여 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 클래스의 새 인스턴스를 초기화합니다. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | 지정된 글꼴 크기와 글꼴 스타일을 사용하여 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 클래스의 새 인스턴스를 초기화합니다. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | 기본 글꼴 설정과 지정된 글꼴 스타일을 사용하여 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getField()](#getField--) | 스타일이 적용될 필드를 가져옵니다. |
| [getItemType()](#getItemType--) | 텍스트 항목 유형을 반환합니다. |
| [getRowUid()](#getRowUid--) | 행 고유 ID를 가져옵니다. |
| [setField(int value)](#setField-int-) | 스타일이 적용될 필드를 설정합니다. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


[TableTextStyle](../../com.aspose.tasks/tabletextstyle) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowUid | int | 지정된 행 고유 ID. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


지정된 글꼴을 사용하여 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowUid | int | 지정된 행 고유 ID. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 텍스트 스타일이 기반하는 글꼴. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


지정된 글꼴 크기와 글꼴 스타일을 사용하여 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowUid | int | 지정된 행 고유 ID. |
| fontSize | float | 텍스트 스타일이 기반하는 글꼴의 크기. |
| fontStyle | int | 글꼴 스타일. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


기본 글꼴 설정과 지정된 글꼴 스타일을 사용하여 [TableTextStyle](../../com.aspose.tasks/tabletextstyle) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowUid | int | 지정된 행 고유 ID. |
| fontStyle | int | 글꼴 스타일. |

### getField() {#getField--}
```
public final int getField()
```


스타일이 적용될 필드를 가져옵니다. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - 스타일이 적용될 필드.
### getItemType() {#getItemType--}
```
public int getItemType()
```


텍스트 항목 유형을 반환합니다.

**Returns:**
int - TextItemType 열거형 값.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


행 고유 ID를 가져옵니다.

--------------------

뷰의 모든 행에 스타일이 적용되는 경우 -1을 반환합니다.

**Returns:**
int - 행 고유 ID.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


스타일이 적용될 필드를 설정합니다. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 스타일이 적용될 필드. |

