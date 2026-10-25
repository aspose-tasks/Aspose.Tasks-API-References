---
title: "ProjectView"
second_title: "Aspose.Tasks for Java API Reference"
description: "Projects view 클래스"
type: docs
weight: 228
url: /ko/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

프로젝트 뷰 클래스
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | 새로운 [ProjectView](../../com.aspose.tasks/projectview) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getColumns()](#getColumns--) | 프로젝트 뷰 열을 가져옵니다. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Uid, 작업 이름, 리소스 이름, 작업량 및 기간 할당 열을 포함합니다. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | id, 표시기, 이름, 기간, 시작 및 종료 작업 열을 포함합니다. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Uid, 리소스 이름, 유형, 재료 라벨, 이니셜, 그룹, 최대 단위, 표준 요금, 초과 근무 요금, 사용당 비용, 발생 시점, 기본 캘린더 및 코드 리소스 열을 포함합니다. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Uid, 이름, 시작, 종료 및 작업 리소스 열을 포함합니다. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | id, 표시기, 이름, 기간, 시작, 종료, 선행 작업 및 리소스 이름 작업 열을 포함합니다. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


새로운 [ProjectView](../../com.aspose.tasks/projectview) 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 열 | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | 뷰 열의 목록입니다. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


프로젝트 뷰 열을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - 프로젝트 뷰 열.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Uid, 작업 이름, 리소스 이름, 작업량 및 기간 할당 열을 포함합니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


id, 표시기, 이름, 기간, 시작 및 종료 작업 열을 포함합니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Uid, 리소스 이름, 유형, 재료 라벨, 이니셜, 그룹, 최대 단위, 표준 요금, 초과 근무 요금, 사용당 비용, 발생 시점, 기본 캘린더 및 코드 리소스 열을 포함합니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Uid, 이름, 시작, 종료 및 작업 리소스 열을 포함합니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


id, 표시기, 이름, 기간, 시작, 종료, 선행 작업 및 리소스 이름 작업 열을 포함합니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
