---
title: "Sınıf CsvOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.CsvOptions sınıfı. Projeyi CSV'ye kaydederken ek seçenekler belirtmeye olanak tanır."
type: docs
weight: 1980
url: /tr/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Projeyi CSV'ye kaydederken ek seçenekleri belirtmeye izin verir.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CsvOptions](csvoptions/)() | `CsvOptions` sınıfının yeni bir örneğini başlatır; bu örnek, projeyi CSV formatında kaydetmekte kullanılabilir. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Kaydedilecek bir veri kategorisini alır veya ayarlar. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | CSV'yi kaydetmek için bir kodlamayı alır veya ayarlar. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Başlıkların dahil edilip edilmeyeceğini gösteren bir değeri alır veya ayarlar (varsayılan değer TRUE'dır). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı şemalarında renderlanan görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Metin sınırlayıcısını alır veya ayarlar. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Görünüm sütunlarının ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) bir listesini alır veya ayarlar ve XLSX formatında kaydetmek için kullanır. Ayarlanmamışsa varsayılan sütunlar kaydedilir. |

## Örnekler

Bir projeyi CSV dosyası olarak kaydetmek için &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; kullanımını gösterir.

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


