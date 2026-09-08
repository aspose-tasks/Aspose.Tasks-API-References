---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "FieldHelper 메서드. 특정 필드의 기본 제목을 반환합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

특정 필드의 기본 제목을 반환합니다.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 필드 | 필드 | 기본 제목을 가져올 필드. |

### 반환 값

필드가 MS Project 뷰에 표시될 수 있는 경우 해당 필드의 기본 제목이며, 그렇지 않으면 null입니다.

## 예제

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


