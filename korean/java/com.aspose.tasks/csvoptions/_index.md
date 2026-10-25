---
title: "CsvOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트를 CSV로 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 56
url: /ko/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

프로젝트를 CSV로 저장할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | CSV 형식으로 프로젝트를 저장하는 데 사용할 수 있는 [CsvOptions](../../com.aspose.tasks/csvoptions) 클래스를 새 인스턴스로 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | 저장될 데이터 카테고리를 가져옵니다. |
| [getEncoding()](#getEncoding--) | CSV를 저장할 인코딩을 가져옵니다. |
| [getIncludeHeaders()](#getIncludeHeaders--) | 헤더를 포함할지 여부를 나타내는 값을 가져옵니다(기본값은 TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | 텍스트 구분자를 가져옵니다. |
| [getView()](#getView--) | XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록을 가져옵니다. |
| [setDataCategory(int value)](#setDataCategory-int-) | 저장될 데이터 카테고리를 설정합니다. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | CSV를 저장할 인코딩을 설정합니다. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | 헤더를 포함할지 여부를 나타내는 값을 설정합니다(기본값은 TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | 텍스트 구분자를 설정합니다. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록을 설정합니다. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


CSV 형식으로 프로젝트를 저장하는 데 사용할 수 있는 [CsvOptions](../../com.aspose.tasks/csvoptions) 클래스를 새 인스턴스로 초기화합니다.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


저장될 데이터 카테고리를 가져옵니다.

**Returns:**
int - 저장될 데이터 카테고리입니다.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


CSV를 저장할 인코딩을 가져옵니다.

**Returns:**
java.nio.charset.Charset - CSV를 저장할 인코딩입니다.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


헤더를 포함할지 여부를 나타내는 값을 가져옵니다(기본값은 TRUE).

**Returns:**
boolean - 헤더를 포함할지 여부를 나타내는 값입니다 (기본값은 TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


텍스트 구분자를 가져옵니다.

**Returns:**
int - 텍스트 구분자입니다.
### getView() {#getView--}
```
public final ProjectView getView()
```


XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록을 가져옵니다. 설정하지 않으면 기본 열이 저장됩니다.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


저장될 데이터 카테고리를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 저장될 데이터 카테고리입니다. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


CSV를 저장할 인코딩을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.nio.charset.Charset | CSV를 저장할 인코딩입니다. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


헤더를 포함할지 여부를 나타내는 값을 설정합니다(기본값은 TRUE).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 헤더를 포함할지 여부를 나타내는 값입니다 (기본값은 TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


텍스트 구분자를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 텍스트 구분자입니다. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록을 설정합니다. 설정하지 않으면 기본 열이 저장됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | XLSX 형식으로 저장할 보기 열([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) 목록입니다. |

