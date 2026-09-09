---
title: "CsvOptions.View"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CsvOptions özelliği. XLSX formatında kaydetmek için görüntü sütunları GanttChartColumn listesini alır veya ayarlar. Ayarlanmamışsa varsayılan sütunlar kaydedilir."
type: docs
weight: 60
url: /tr/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

XLSX formatında kaydetmek için görüntü sütunları ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) listesini alır veya ayarlar. Ayarlanmamışsa varsayılan sütunlar kaydedilir.

```csharp
public ProjectView View { get; set; }
```

## Örnekler

Varsayılan Gantt Şeması sütunlarını almak için &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; nasıl kullanılacağını gösterir ve

```csharp
// bunları bir CSV dosyasına kaydeder.
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

### Ayrıca Bakınız

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


