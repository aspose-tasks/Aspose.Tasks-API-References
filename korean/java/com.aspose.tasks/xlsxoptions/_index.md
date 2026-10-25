---
title: "XlsxOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 페이지를 XLSX로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 368
url: /ko/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

프로젝트 페이지를 XLSX로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | [XlsxOptions](../../com.aspose.tasks/xlsxoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 프로젝트를 XLSX 형식으로 저장하는 데 사용할 수 있습니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | 렌더링할 할당 보기 열 목록을 가져옵니다 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | 결과 XLSX 파일의 인코딩을 가져옵니다. |
| [getResourceView()](#getResourceView--) | 렌더링할 리소스 보기 열 목록을 가져옵니다 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록을 가져옵니다. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | 렌더링할 할당 보기 열 목록을 설정합니다 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | 결과 XLSX 파일의 인코딩을 설정합니다. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | 렌더링할 리소스 보기 열 목록을 설정합니다 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록을 설정합니다. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


[XlsxOptions](../../com.aspose.tasks/xlsxoptions) 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 프로젝트를 XLSX 형식으로 저장하는 데 사용할 수 있습니다.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


렌더링할 할당 보기 열 목록을 가져옵니다 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


결과 XLSX 파일의 인코딩을 가져옵니다. 기본값은 java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8입니다.

**Returns:**
java.nio.charset.Charset - 결과 XLSX 파일의 인코딩.
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


XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록을 가져옵니다. 설정하지 않으면 기본 열이 저장됩니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


렌더링할 할당 보기 열 목록을 설정합니다 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 렌더링할 할당 보기 열 목록 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


결과 XLSX 파일의 인코딩을 설정합니다. 기본값은 java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.nio.charset.Charset | 결과 XLSX 파일의 인코딩. |

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


XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록을 설정합니다. 설정하지 않으면 기본 열이 저장됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록입니다. |

