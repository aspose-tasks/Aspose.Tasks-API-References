---
title: "GanttChartColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "Projects view 클래스"
type: docs
weight: 111
url: /ko/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

프로젝트 뷰 클래스
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | 새 인스턴스를 초기화합니다 GanttChartColumn 클래스. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | 새 인스턴스를 초기화합니다 GanttChartColumn 클래스. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | 새 인스턴스를 초기화합니다 GanttChartColumn 클래스. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | 새 인스턴스를 초기화합니다 GanttChartColumn 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | 현재 작업을 열 텍스트로 변환합니다. |
| [getField()](#getField--) | 열 필드를 반환합니다. |
| [setField(int value)](#setField-int-) | 열 필드를 설정합니다. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


새 인스턴스를 초기화합니다 GanttChartColumn 클래스.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 열 이름입니다. |
| width | int | 열의 너비(픽셀 단위)입니다. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | 작업 데이터를 열 텍스트로 변환하는 변환기. |
| 필드 | int | 열 필드. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


새 인스턴스를 초기화합니다 GanttChartColumn 클래스.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 열 이름입니다. |
| width | int | 열의 너비(픽셀 단위)입니다. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | 작업 데이터를 열 텍스트로 변환하는 변환기. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


새 인스턴스를 초기화합니다 GanttChartColumn 클래스.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| width | int | 픽셀 단위의 열 너비. |
| 필드 | int | 열 필드. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


새 인스턴스를 초기화합니다 GanttChartColumn 클래스.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 열 이름입니다. |
| width | int | 픽셀 단위의 열 너비. |
| 필드 | int | 열 필드. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


현재 작업을 열 텍스트로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 현재 작업입니다. |

**Returns:**
java.lang.String - 열 텍스트.
### getField() {#getField--}
```
public int getField()
```


열 필드를 반환합니다. `Field`.

**Returns:**
int - 열 필드 값.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


열 필드를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 열 필드 값. |

