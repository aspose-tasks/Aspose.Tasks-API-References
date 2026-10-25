---
title: "ProgressLines"
second_title: "Aspose.Tasks for Java API Reference"
description: "간트 차트 보기에서 진행 라인을 나타냅니다."
type: docs
weight: 219
url: /ko/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

간트 차트 보기에서 진행 라인을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | 진행 라인을 표시할 시작 날짜를 가져옵니다. |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | 프로젝트 시작 날짜부터 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다. |
| [getDateFormat()](#getDateFormat--) | 날짜 형식을 가져옵니다 ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | 현재 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다. |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | 반복 간격으로 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다. |
| [getDisplaySelected()](#getDisplaySelected--) | 선택한 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다. |
| [getFont()](#getFont--) | 진행 라인 레이블에 사용되는 글꼴을 가져옵니다. |
| [getLineColor()](#getLineColor--) | 현재 진행 라인의 선 색상을 가져옵니다. |
| [getLinePattern()](#getLinePattern--) | 현재 진행 라인의 선 패턴을 가져옵니다. |
| [getOtherLineColor()](#getOtherLineColor--) | 다른 진행 라인의 색상을 가져옵니다. |
| [getOtherLinePattern()](#getOtherLinePattern--) | 다른 진행 라인의 선 패턴을 가져옵니다. |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | 다른 진행 지점의 색상을 가져옵니다. |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | 다른 진행 라인의 진행 지점 모양을 가져옵니다. |
| [getProgressPointColor()](#getProgressPointColor--) | 진행 지점의 색상을 가져옵니다. |
| [getProgressPointShape()](#getProgressPointShape--) | 진행 지점 모양을 가져옵니다. |
| [getRecurringInterval()](#getRecurringInterval--) | 반복 간격을 가져옵니다. |
| [getSelectedDates()](#getSelectedDates--) | 진행 라인을 표시할 선택된 날짜 목록을 가져옵니다. |
| [getShowDate()](#getShowDate--) | 각 진행 라인에 날짜를 표시할지 여부를 나타내는 값을 가져옵니다. |
| [isBaselinePlan()](#isBaselinePlan--) | 기준 계획 또는 실제에 대한 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다. |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | 기준 계획 또는 실제에 대한 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다. |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | 진행 라인을 표시할 시작 날짜를 설정합니다. |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | 프로젝트 시작 날짜의 시작부터 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다. |
| [setDateFormat(int value)](#setDateFormat-int-) | 날짜 형식을 설정합니다 ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | 현재 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다. |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | 반복 간격에 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다. |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | 선택된 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | 진행 라인 레이블에 사용할 글꼴을 설정합니다. |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | 현재 진행 라인의 선 색상을 설정합니다. |
| [setLinePattern(int value)](#setLinePattern-int-) | 현재 진행 라인의 선 패턴을 설정합니다. |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | 다른 진행 라인의 색상을 설정합니다. |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | 다른 진행 라인의 선 패턴을 설정합니다. |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | 다른 진행 지점의 색상을 설정합니다. |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | 다른 진행 라인의 진행 지점 모양을 설정합니다. |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | 진행 지점의 색상을 설정합니다. |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | 진행 지점 모양을 설정합니다. |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | 반복 간격을 설정합니다. |
| [setShowDate(boolean value)](#setShowDate-boolean-) | 각 진행 라인에 대한 날짜 표시 여부를 나타내는 값을 설정합니다. |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


진행 라인을 표시할 시작 날짜를 가져옵니다.

**Returns:**
java.util.Date - 진행 라인을 표시할 시작 날짜입니다.
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


프로젝트 시작 날짜부터 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 프로젝트 시작 날짜부터 진행 라인을 표시할지 여부를 나타내는 값입니다.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


날짜 형식을 가져옵니다 ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - 날짜 형식 ([DateLabel](../../com.aspose.tasks/datelabel))입니다.
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


현재 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 현재 날짜에 진행 라인을 표시할지 여부를 나타내는 값입니다.
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


반복 간격으로 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 반복 간격에 진행 라인을 표시할지 여부를 나타내는 값입니다.
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


선택한 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 선택된 날짜에 진행 라인을 표시할지 여부를 나타내는 값입니다.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


진행 라인 레이블에 사용되는 글꼴을 가져옵니다.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


현재 진행 라인의 선 색상을 가져옵니다.

**Returns:**
java.awt.Color - 현재 진행 라인의 선 색상입니다.
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


현재 진행 라인의 선 패턴을 가져옵니다. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - 현재 진행 라인의 선 패턴입니다.
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


다른 진행 라인의 색상을 가져옵니다.

**Returns:**
java.awt.Color - 다른 진행 라인의 색상입니다.
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


다른 진행 라인의 선 패턴을 가져옵니다.

**Returns:**
int - 다른 진행 라인의 선 패턴입니다.
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


다른 진행 지점의 색상을 가져옵니다.

**Returns:**
java.awt.Color - 다른 진행 지점의 색상입니다.
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


다른 진행 라인의 진행 지점 모양을 가져옵니다.

**Returns:**
int - 다른 진행 라인의 진행 지점 모양입니다.
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


진행 지점의 색상을 가져옵니다.

**Returns:**
java.awt.Color - 진행 지점의 색상입니다.
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


진행 지점 모양을 가져옵니다. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - 진행 지점 모양입니다.
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


반복 간격을 가져옵니다. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


진행 라인을 표시할 선택된 날짜 목록을 가져옵니다.

**Returns:**
java.util.List&lt;java.util.Date&gt; - 진행 라인을 표시할 선택된 날짜 목록입니다.
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


각 진행 라인에 날짜를 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 각 진행 라인에 날짜를 표시할지 여부를 나타내는 값입니다.
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


기준 계획 또는 실제에 대한 진행 라인을 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 기준 계획 또는 실제에 대한 진행 라인을 표시할지 여부를 나타내는 값입니다.
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


기준 계획 또는 실제에 대한 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 기준 계획 또는 실제에 대한 진행 라인을 표시할지 여부를 나타내는 값입니다. |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


진행 라인을 표시할 시작 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 진행 라인을 표시할 시작 날짜입니다. |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


프로젝트 시작 날짜의 시작부터 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트 시작 날짜부터 진행 라인을 표시할지 여부를 나타내는 값입니다. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


날짜 형식을 설정합니다 ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | 날짜 형식 ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


현재 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 현재 날짜에 진행 라인을 표시할지 여부를 나타내는 값. |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


반복 간격에 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 반복 간격에 진행 라인을 표시할지 여부를 나타내는 값. |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


선택된 날짜에 진행 라인을 표시할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 선택된 날짜에 진행 라인을 표시할지 여부를 나타내는 값. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


진행 라인 레이블에 사용할 글꼴을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | 진행 라인 레이블에 사용되는 글꼴. |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


현재 진행 라인의 선 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 현재 진행 라인의 선 색상. |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


현재 진행 라인의 선 패턴을 설정합니다. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 현재 진행 라인의 선 패턴. |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


다른 진행 라인의 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 다른 진행 라인의 색상. |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


다른 진행 라인의 선 패턴을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 다른 진행 라인의 선 패턴. |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


다른 진행 지점의 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 다른 진행 지점의 색상. |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


다른 진행 라인의 진행 지점 모양을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 다른 진행 라인의 진행 지점 모양. |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


진행 지점의 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 진행 지점의 색상. |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


진행 지점 모양을 설정합니다. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 진행 지점 모양. |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


반복 간격을 설정합니다. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | 반복 간격. |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


각 진행 라인에 대한 날짜 표시 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 각 진행 라인에 날짜를 표시할지 여부를 나타내는 값. |

