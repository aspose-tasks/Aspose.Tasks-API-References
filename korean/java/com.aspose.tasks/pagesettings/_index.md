---
title: "PageSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 보기 페이지에 대한 인쇄 설정을 나타냅니다."
type: docs
weight: 181
url: /ko/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

프로젝트 보기 페이지에 대한 인쇄 설정을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PageSettings()](#PageSettings--) | 새로운 [PageSettings](../../com.aspose.tasks/pagesettings) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | 정규 크기의 지정된 백분율(`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-)))에 맞게 인쇄를 조정할지 여부를 나타내는 값을 가져옵니다. |
| [getFirstPageNumber()](#getFirstPageNumber--) | 인쇄할 첫 페이지 번호를 가져옵니다. |
| [getPagesInHeight()](#getPagesInHeight--) | 인쇄할 높이 방향 페이지 수를 가져옵니다. |
| [getPagesInWidth()](#getPagesInWidth--) | 인쇄할 너비 방향 페이지 수를 가져옵니다. |
| [getPaperSize()](#getPaperSize--) | 용지 크기를 가져옵니다. |
| [getPaperSizeId()](#getPaperSizeId--) | PrinterPaperSize 값 중 하나 또는 사용자 지정 페이지 크기 ID를 나타내는 정수를 가져옵니다. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | 인쇄를 조정할 정규 크기의 백분율을 가져옵니다. |
| [isPortrait()](#isPortrait--) | 페이지 방향이 세로인지 여부를 나타내는 값을 가져옵니다; 페이지 방향이 가로인 경우 false를 반환합니다. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | 정규 크기의 지정된 백분율(`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-)))에 맞게 인쇄를 조정할지 여부를 나타내는 값을 설정합니다. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | 인쇄할 첫 페이지 번호를 설정합니다. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | 인쇄할 높이 방향 페이지 수를 설정합니다. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | 인쇄할 너비 방향 페이지 수를 설정합니다. |
| [setPaperSize(int value)](#setPaperSize-int-) | 용지 크기를 설정합니다. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | PrinterPaperSize 값 중 하나 또는 사용자 지정 페이지 크기 ID를 나타내는 정수를 설정합니다. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | 인쇄를 조정할 정규 크기의 백분율을 설정합니다. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | 페이지 방향이 세로인지 여부를 나타내는 값을 설정합니다; 페이지 방향이 가로인 경우 false를 반환합니다. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


새로운 [PageSettings](../../com.aspose/tasks/pagesettings) 클래스 인스턴스를 초기화합니다. 프로젝트 뷰 페이지의 인쇄 설정을 나타냅니다.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


정규 크기의 지정된 백분율(`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-)))에 맞게 인쇄를 조정할지 여부를 나타내는 값을 가져옵니다.

--------------------

프로젝트가 HTML 형식으로 렌더링될 때는 적용되지 않습니다.

**Returns:**
boolean - 정규 크기의 지정된 백분율(`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-)))에 맞게 인쇄를 조정할지 여부를 나타내는 값.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


인쇄할 첫 페이지 번호를 가져옵니다.

**Returns:**
short - 인쇄할 첫 페이지 번호.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


인쇄할 높이 방향 페이지 수를 가져옵니다.

**Returns:**
int - 인쇄할 높이 방향 페이지 수.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


인쇄할 너비 방향 페이지 수를 가져옵니다.

**Returns:**
int - 인쇄할 너비 방향 페이지 수.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


용지 크기를 가져옵니다. [PrinterPaperSize](../../com.aspose/tasks/printerpapersize) 열거형의 값 중 하나일 수 있습니다.

**Returns:**
int - 용지 크기.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


PrinterPaperSize 값 중 하나 또는 사용자 지정 페이지 크기 ID를 나타내는 정수를 가져옵니다. 이 값은 OS 설정에서 PaperSize를 가져오는 데 사용할 수 있습니다 ().

**Returns:**
int - PrinterPaperSize 값 중 하나 또는 사용자 정의 페이지 크기 ID를 나타내는 정수입니다.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


인쇄를 조정할 정규 크기의 백분율을 가져옵니다.

**Returns:**
int - 인쇄를 조정할 정상 크기의 백분율입니다.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


페이지 방향이 세로인지 여부를 나타내는 값을 가져옵니다; 페이지 방향이 가로인 경우 false를 반환합니다.

--------------------

SaveOptions.getPageSize() == PageSize.DefinedInView 일 때 렌더링 중에 적용됩니다.

**Returns:**
boolean - 페이지 방향이 세로인지 여부를 나타내는 값이며, 가로인 경우 false를 반환합니다.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


정규 크기의 지정된 백분율(`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-)))에 맞게 인쇄를 조정할지 여부를 나타내는 값을 설정합니다.

--------------------

프로젝트가 HTML 형식으로 렌더링될 때는 적용되지 않습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | boolean | 정해진 백분율(`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) 로 정상 크기에 맞게 인쇄를 조정할지 여부를 나타내는 값입니다. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


인쇄할 첫 페이지 번호를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | short | 인쇄를 위한 첫 페이지 번호입니다. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


인쇄할 높이 방향 페이지 수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 인쇄될 높이 방향 페이지 수입니다. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


인쇄할 너비 방향 페이지 수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 인쇄될 너비 방향 페이지 수입니다. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


용지 크기를 설정합니다. [PrinterPaperSize](../../com.aspose.tasks/printerpapersize) 열거형의 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 용지 크기입니다. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


PrinterPaperSize 값 중 하나 또는 사용자 정의 페이지 크기 ID를 나타내는 정수를 설정합니다. 이 값은 OS 설정에서 PaperSize를 가져오는 데 사용할 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | PrinterPaperSize 값 중 하나 또는 사용자 정의 페이지 크기 ID를 나타내는 정수입니다. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


인쇄를 조정할 정규 크기의 백분율을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 인쇄를 조정할 정상 크기의 백분율입니다. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


페이지 방향이 세로인지 여부를 나타내는 값을 설정합니다; 페이지 방향이 가로인 경우 false를 반환합니다.

--------------------

SaveOptions.getPageSize() == PageSize.DefinedInView 일 때 렌더링 중에 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 페이지 방향이 세로인지 여부를 나타내는 값이며, 가로인 경우 false를 반환합니다. |

