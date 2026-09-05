---
title: "SaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "특정 형식으로 프로젝트를 저장할 때 사용자가 추가 옵션을 지정할 수 있도록 하는 클래스들을 위한 추상 기본 클래스입니다."
type: docs
weight: 274
url: /ko/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

특정 형식으로 프로젝트를 저장할 때 사용자가 추가 옵션을 지정할 수 있도록 하는 클래스들을 위한 추상 기본 클래스입니다.

--------------------

SaveOptions 클래스에서 파생된 모든 클래스의 인스턴스는 문서를 저장할 때 사용자가 사용자 지정 옵션을 정의할 수 있도록 스트림 Save 또는 문자열 Save 오버로드에 전달됩니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | 프로젝트 뷰에 표시되는 [BarStyle](../../com.aspose.tasks/barstyle) 클래스 인스턴스 목록을 가져옵니다. |
| [getCustomPageSize()](#getCustomPageSize--) | 포인트 단위(1 포인트 = 1/72 인치)의 사용자 정의 페이지 크기를 가져옵니다. |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | 비작업 시간이 그려져야 하는지 여부를 나타내는 값을 가져옵니다(기본값은 TRUE). |
| [getEndDate()](#getEndDate--) | 렌더링을 종료할 날짜를 가져옵니다. |
| [getFitContent()](#getFitContent--) | 행 높이를 내용에 맞게 늘려야 하는지 여부를 나타내는 값을 가져옵니다. |
| [getGridlines()](#getGridlines--) | 프로젝트 뷰에 표시되는 [Gridline](../../com.aspose.tasks/gridline) 목록을 가져옵니다. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | 범례를 렌더링하는 방법을 정의하는 값을 가져옵니다. |
| [getLegendItems()](#getLegendItems--) | 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 가져옵니다. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져옵니다(기본값은 FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | 비작업 시간 색상을 가져옵니다. |
| [getPageCount()](#getPageCount--) | 프로젝트 페이지 수를 가져옵니다. |
| [getPageSize()](#getPageSize--) | 렌더링될 페이지 크기를 가져옵니다(기본값은 PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | 문서가 저장될 `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))을 가져옵니다. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링될지 여부를 나타내는 값을 가져옵니다. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | 요약 작업 막대의 하위 작업이 표시될지 여부를 나타내는 값을 가져옵니다. |
| [getStartDate()](#getStartDate--) | 렌더링을 시작할 날짜를 가져옵니다. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | 작업 링크 렌더링의 일부 측면을 사용자 지정하는 데 사용할 수 있는 콜백을 가져옵니다. |
| [getTextStyles()](#getTextStyles--) | 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 가져옵니다. |
| [getTimescale()](#getTimescale--) | `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 값을 가져옵니다. 이 값은 프로젝트가 그래픽 형식으로 저장될 때 타임스케일(있는 경우)이 어떻게 렌더링되는지를 제어합니다. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방법을 정의하는 동작을 가져옵니다. |
| [getUseGradientBrush()](#getUseGradientBrush--) | 간트 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져옵니다. |
| [getView()](#getView--) | 렌더링할 뷰 열 목록을 가져옵니다 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | 렌더링할 뷰(`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)))를 가져옵니다. |
| [isPortrait()](#isPortrait--) | 페이지 방향이 세로인지 여부를 나타내는 값을 가져옵니다; 페이지 방향이 가로인 경우 false를 반환합니다. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | 프로젝트 뷰에 표시되는 [BarStyle](../../com.aspose.tasks/barstyle) 클래스 인스턴스 목록을 설정합니다. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | 포인트 단위(1 포인트 = 1/72 인치)의 사용자 정의 페이지 크기를 설정합니다. |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | 비작업 시간을 그릴지 여부를 나타내는 값을 설정합니다(기본값은 TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | 렌더링을 종료할 날짜를 설정합니다. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 설정합니다. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | 프로젝트 뷰에 표시되는 [Gridline](../../com.aspose.tasks/gridline) 목록을 설정합니다. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | 범례를 렌더링하는 방법을 정의하는 값을 설정합니다. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 설정합니다. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 설정합니다(기본값은 FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | 비작업 시간 색상을 설정합니다. |
| [setPageSize(int value)](#setPageSize-int-) | 렌더링될 페이지 크기를 설정합니다(기본값은 PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | 페이지 방향이 세로인지 여부를 나타내는 값을 설정합니다; 페이지 방향이 가로인 경우 false를 반환합니다. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | 문서가 저장될 `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))을 설정합니다. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링될지 여부를 나타내는 값을 설정합니다. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | 요약 작업 막대의 하위 작업을 표시할지 여부를 나타내는 값을 설정합니다. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | 렌더링을 시작할 날짜를 설정합니다. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | 작업 링크 렌더링의 일부 측면을 사용자 지정하는 데 사용할 수 있는 콜백을 설정합니다. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 설정합니다. |
| [setTimescale(int value)](#setTimescale-int-) | 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(존재하는 경우)이 렌더링되는 방식을 제어하는 데 사용되는 `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 값을 설정합니다. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 설정합니다. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | 간트 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 설정합니다. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | 렌더링할 뷰 열 목록을 설정합니다 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | 렌더링할 뷰 (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)))를 설정합니다. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


프로젝트 뷰에 표시되는 [BarStyle](../../com.aspose.tasks/barstyle) 클래스 인스턴스 목록을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - 프로젝트 뷰에 나타나는 [BarStyle](../../com.aspose.tasks/barstyle) 클래스 인스턴스 목록입니다.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


포인트 단위(1 포인트 = 1/72 인치)의 사용자 정의 페이지 크기를 가져옵니다.

**Returns:**
java.awt.geom.Dimension2D - 포인트 단위의 사용자 지정 페이지 크기입니다 (1 포인트 = 1/72 인치).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


비작업 시간이 그려져야 하는지 여부를 나타내는 값을 가져옵니다(기본값은 TRUE).

**Returns:**
boolean - 비작업 시간을 그릴지 여부를 나타내는 값입니다 (기본값은 TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


렌더링을 종료할 날짜를 가져옵니다.

**Returns:**
java.util.Date - 렌더링을 종료할 날짜입니다.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


행 높이를 내용에 맞게 늘려야 하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값입니다.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


프로젝트 뷰에 표시되는 [Gridline](../../com.aspose.tasks/gridline) 목록을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - 프로젝트 뷰에 나타나는 [Gridline](../../com.aspose.tasks/gridline) 목록입니다.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


범례를 렌더링하는 방식을 정의하는 값을 가져옵니다. 기본값은 LegendDrawingOptions.OnEveryPage입니다.

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Returns:**
int - 범례를 렌더링하는 방식을 정의하는 값입니다.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 가져옵니다. null인 경우 기본 항목이 렌더링됩니다.

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Returns:**
com.aspose.tasks.PageLegendItem[] - 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열입니다.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 가져옵니다(기본값은 FALSE).

**Returns:**
boolean - 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값입니다 (기본값은 FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


비작업 시간 색상을 가져옵니다.

**Returns:**
java.awt.Color - 비작업 시간 색상입니다.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


프로젝트 페이지 수를 가져옵니다.

**Returns:**
int - 프로젝트 페이지 수입니다.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


렌더링될 페이지 크기를 가져옵니다(기본값은 PageSize.A4).

**Returns:**
int - 렌더링될 페이지 크기입니다 (기본값은 PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


문서가 저장될 `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))을 가져옵니다.

**Returns:**
int - 문서가 저장될 `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))을 나타내는 값입니다.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링될지 여부를 나타내는 값을 가져옵니다. 페이지 크기가 변경되어 렌더링된 프로젝트가 한 페이지에 맞게 됩니다.

**Returns:**
boolean - 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링되는지를 나타내는 값.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


요약 작업 막대에 하위 작업이 표시되어야 하는지를 나타내는 값을 가져옵니다. 하위 작업의 경우, Rollup 필드는 하위 작업 간트 막대의 정보가 요약 작업 막대로 롤업되는지를 나타냅니다. 요약 작업의 경우, Rollup 필드는 요약 작업 막대가 롤업된 막대를 표시하는지를 나타냅니다. 하위 작업이 롤업되도록 하려면 요약 작업에 대한 Rollup 필드를 Yes 로 설정해야 합니다.

--------------------

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Returns:**
boolean - 요약 작업 막대에 하위 작업이 표시되어야 하는지를 나타내는 값.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


렌더링을 시작할 날짜를 가져옵니다.

**Returns:**
java.util.Date - 렌더링을 시작할 날짜.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


작업 링크 렌더링의 일부 측면을 사용자 지정하는 데 사용할 수 있는 콜백을 가져옵니다.

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 가져옵니다.

--------------------

이 스타일은 GanttCharView.setTextStyles 로 정의된 스타일을 재정의합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


`Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 값을 가져옵니다. 이 값은 프로젝트가 그래픽 형식으로 저장될 때 타임스케일(있는 경우)이 어떻게 렌더링되는지를 제어합니다.

**Returns:**
int - `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 값으로, 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(존재하는 경우)이 어떻게 렌더링되는지를 제어하는 데 사용됩니다.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방법을 정의하는 동작을 가져옵니다.

**Returns:**
int - 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


간트 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져옵니다.

--------------------

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Returns:**
boolean - 간트 차트를 렌더링할 때 그라디언트 브러시를 사용할지를 나타내는 값.
### getView() {#getView--}
```
public final ProjectView getView()
```


렌더링할 뷰 열의 목록을 가져옵니다 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). 설정되지 않으면 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 재정의합니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


렌더링할 뷰 (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)))를 가져옵니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장될 뷰를 명시적으로 지정할 수 있습니다. 이 속성이 설정된 경우, 프로젝트 저장 시 [PresentationFormat](../../com.aspose.tasks/presentationformat) 속성이 무시됩니다. 뷰는 다음 화면 중 하나에서 선택해야 합니다 ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


페이지 방향이 세로인지 여부를 나타내는 값을 가져옵니다; 페이지 방향이 가로인 경우 false를 반환합니다.

--------------------

SaveOptions.getPageSize() == PageSize.DefinedInView인 경우 적용되지 않습니다. 이 경우 [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--)가 대신 사용됩니다. [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--)가 설정된 경우에도 적용되지 않습니다.

**Returns:**
boolean - 페이지 방향이 세로인지 여부를 나타내는 값이며, 가로인 경우 false를 반환합니다.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


프로젝트 뷰에 표시되는 [BarStyle](../../com.aspose.tasks/barstyle) 클래스 인스턴스 목록을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | 프로젝트 뷰에 표시되는 [BarStyle](../../com.aspose.tasks/barstyle) 클래스 인스턴스 목록. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


포인트 단위(1 포인트 = 1/72 인치)의 사용자 정의 페이지 크기를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.geom.Dimension2D | 포인트 단위의 사용자 정의 페이지 크기 (1 포인트 = 1/72 인치). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


비작업 시간을 그릴지 여부를 나타내는 값을 설정합니다(기본값은 TRUE).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 비작업 시간을 그릴지 여부를 나타내는 값 (기본값은 TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


렌더링을 종료할 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 렌더링을 종료할 날짜. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


프로젝트 뷰에 표시되는 [Gridline](../../com.aspose.tasks/gridline) 목록을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | 프로젝트 뷰에 표시되는 [Gridline](../../com.aspose.tasks/gridline) 목록. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


범례를 렌더링하는 방법을 정의하는 값을 설정합니다. 기본값은 LegendDrawingOptions.OnEveryPage입니다.

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 범례를 렌더링하는 방법을 정의하는 값. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열을 설정합니다. null인 경우 기본 항목이 렌더링됩니다.

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | 페이지 범례에 렌더링될 막대를 정의하는 PageLegendItem 배열. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


중요 작업을 빨간색으로 표시할지 여부를 나타내는 값을 설정합니다(기본값은 FALSE).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 중요 작업을 빨간색으로 표시할지 여부를 나타내는 값 (기본값은 FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


비작업 시간 색상을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | 비작업 시간 색상. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


렌더링될 페이지 크기를 설정합니다(기본값은 PageSize.A4).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 렌더링될 페이지 크기 (기본값은 PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


페이지 방향이 세로인지 여부를 나타내는 값을 설정합니다; 페이지 방향이 가로인 경우 false를 반환합니다.

--------------------

SaveOptions.PageSize == Visualization.PageSize.DefinedInView인 경우 적용되지 않습니다. 이 경우 [PageSettings.setPortrait(boolean)](../../com.aspose/tasks/pagesettings\#setPortrait-boolean-)가 대신 사용됩니다. [getCustomPageSize()](../../com.aspose/tasks/saveoptions\#getCustomPageSize--)가 설정된 경우에도 적용되지 않습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 페이지 방향이 세로인지 여부를 나타내는 값이며, 가로인 경우 false를 반환합니다. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


문서가 저장될 `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | 문서가 저장될 `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)). |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링될지 여부를 나타내는 값을 설정합니다. 페이지 크기가 변경되어 렌더링된 프로젝트가 한 페이지에 맞도록 합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트가 그래픽 형식으로 저장될 때 단일 페이지로 렌더링될지 여부를 나타내는 값. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


요약 작업 막대에 있는 하위 작업을 표시할지 여부를 나타내는 값을 설정합니다. 하위 작업의 경우 Rollup 필드는 하위 작업 Gantt 막대의 정보가 요약 작업 막대로 롤업되는지를 나타냅니다. 요약 작업의 경우 Rollup 필드는 요약 작업 막대가 롤업된 막대를 표시하는지를 나타냅니다. 하위 작업이 롤업되도록 하려면 요약 작업에 대한 Rollup 필드를 Yes로 설정해야 합니다.

--------------------

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 요약 작업 막대에 있는 하위 작업을 표시할지 여부를 나타내는 값. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


렌더링을 시작할 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 렌더링을 시작할 날짜. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


작업 링크 렌더링의 일부 측면을 사용자 지정하는 데 사용할 수 있는 콜백을 설정합니다.

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | 작업 링크 렌더링의 일부 측면을 사용자 정의하는 데 사용할 수 있는 콜백. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 설정합니다.

--------------------

이 스타일은 GanttCharView.setTextStyles 로 정의된 스타일을 재정의합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


프로젝트를 그래픽 형식으로 저장할 때 타임스케일(존재하는 경우)이 렌더링되는 방식을 제어하는 데 사용되는 `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 값은 프로젝트를 그래픽 형식으로 저장할 때 타임스케일(존재하는 경우)이 어떻게 렌더링되는지를 제어하는 데 사용됩니다. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방식을 정의하는 동작을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 타임스케일의 오른쪽 끝을 페이지 끝에 맞추는 방법을 정의하는 동작. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


간트 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 설정합니다.

--------------------

간트 차트 뷰가 렌더링될 때만 적용됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Gantt 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


렌더링할 뷰 열의 목록을 설정합니다 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). 설정하지 않으면 작업 ID, 작업 이름, 시작 및 종료만 렌더링됩니다. View와 `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) 속성이 모두 설정된 경우, View의 열이 ViewSettings의 열을 우선합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 렌더링할 뷰 열의 목록 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


렌더링할 뷰 (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)))를 설정합니다. 이 옵션을 사용하여 PDF, HTML 또는 이미지 형식으로 저장될 뷰를 명시적으로 지정할 수 있습니다. 이 속성이 설정된 경우 프로젝트가 저장될 때 [PresentationFormat](../../com.aspose.tasks/presentationformat) 속성이 무시됩니다. 뷰는 다음 화면 중 하나에서 선택해야 합니다 ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | 렌더링할 뷰 (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))). |

