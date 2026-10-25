---
title: "CsvOptions 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.CsvOptions 클래스. 프로젝트를 CSV로 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 1980
url: /ko/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

프로젝트를 CSV로 저장할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [CsvOptions](csvoptions/)() | `CsvOptions` 클래스의 새 인스턴스를 초기화하며, 이를 사용하여 프로젝트를 CSV 형식으로 저장할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | 저장될 데이터 범주를 가져오거나 설정합니다. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | CSV를 저장할 인코딩을 가져오거나 설정합니다. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | 헤더를 포함할지 여부를 나타내는 값을 가져오거나 설정합니다(기본값은 TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | 텍스트 구분자를 가져오거나 설정합니다. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | XLSX 형식으로 저장할 보기 열 목록([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/))을 가져오거나 설정합니다. 설정하지 않으면 기본 열이 저장됩니다. |

## 예제

CSV 파일로 프로젝트를 저장하는 방법을 보여줍니다 &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; 사용

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

기본 Gantt 차트의 열을 가져오기 위해 &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt;을 사용하는 방법을 보여줍니다.

```csharp
// CSV 파일에 저장합니다.
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### 또 보기

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


