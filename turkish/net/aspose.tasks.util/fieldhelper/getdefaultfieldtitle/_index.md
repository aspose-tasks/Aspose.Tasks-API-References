---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "FieldHelper yöntemi. Belirli alanın varsayılan başlığını döndürür."
type: docs
weight: 10
url: /tr/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Belirli alanın varsayılan başlığını döndürür.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alan | Alan | Varsayılan bir başlık almak için alan. |

### Dönüş Değeri

Alan, MS Project görünümünde görüntülenebiliyorsa belirli alanın varsayılan başlığı, aksi takdirde null.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


