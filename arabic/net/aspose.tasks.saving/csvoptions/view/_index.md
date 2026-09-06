---
title: "CsvOptions.View"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CsvOptions. يحصل أو يضبط قائمة بأعمدة العرض GanttChartColumn لحفظها بصيغة XLSX. إذا لم يتم الضبط فسيتم حفظ الأعمدة الافتراضية"
type: docs
weight: 60
url: /ar/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

يحصل أو يضبط قائمة بأعمدة العرض ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) لحفظها بصيغة XLSX. إذا لم يتم الضبط فسيتم حفظ الأعمدة الافتراضية.

```csharp
public ProjectView View { get; set; }
```

## الأمثلة

يوضح كيفية استخدام &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; لأخذ أعمدة مخطط جانت الافتراضي و

```csharp
// احفظها في ملف CSV.
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

### انظر أيضًا

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


