---
title: "Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 페이지를 Spreadsheet2003으로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 280
url: /ko/java/com.aspose.tasks/spreadsheet2003saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class Spreadsheet2003SaveOptions extends SimpleSaveOptions
```

프로젝트 페이지를 Spreadsheet2003으로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Spreadsheet2003SaveOptions()](#Spreadsheet2003SaveOptions--) | 새 인스턴스를 초기화합니다 [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | 렌더링할 할당 보기 열 목록을 가져옵니다 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getResourceView()](#getResourceView--) | 렌더링할 리소스 보기 열 목록을 가져옵니다 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | 저장할 보기 열 목록을 가져옵니다 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | 렌더링할 할당 보기 열 목록을 설정합니다 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | 렌더링할 리소스 보기 열 목록을 설정합니다 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | 저장할 보기 열 목록을 설정합니다 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
### Spreadsheet2003SaveOptions() {#Spreadsheet2003SaveOptions--}
```
public Spreadsheet2003SaveOptions()
```


새 인스턴스를 초기화합니다 [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) 클래스.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


렌더링할 할당 보기 열 목록을 가져옵니다 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


렌더링할 리소스 보기 열 목록을 가져옵니다 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


저장할 보기 열 목록을 가져옵니다 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). 설정되지 않은 경우 기본 열이 저장됩니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


렌더링할 할당 보기 열 목록을 설정합니다 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 렌더링할 할당 보기 열 목록 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


렌더링할 리소스 보기 열 목록을 설정합니다 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 렌더링할 리소스 보기 열 목록 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


저장할 보기 열 목록을 설정합니다 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). 설정되지 않은 경우 기본 열이 저장됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 저장할 보기 열 목록 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

