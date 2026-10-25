---
title: "Sınıf XlsxOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.XlsxOptions sınıfı. Proje sayfalarını XLSX formatına render ederken ek seçenekler belirtmeye olanak tanır."
type: docs
weight: 2270
url: /tr/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Proje sayfalarını XLSX olarak oluştururken ek seçenekler belirtmeye izin verir.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | `XlsxOptions` sınıfının yeni bir örneğini başlatır ve bu, projeyi XLSX formatında kaydetmek için kullanılabilir. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Renderlenecek atama görünümü sütunlarının listesini alır veya ayarlar ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Oluşturulan XLSX dosyasının kodlamasını alır veya ayarlar. Varsayılan değer UTF8'dir. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Renderlenecek kaynak görünümü sütunlarının listesini alır veya ayarlar ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı şemalarında renderlanan görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Görünüm sütunlarının ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) bir listesini alır veya ayarlar ve XLSX formatında kaydetmek için kullanır. Ayarlanmamışsa varsayılan sütunlar kaydedilir. |

## Örnekler

XLSX dosyasına bir projeyi kaydetmenin, &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt; seçeneklerini kullanarak nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// İstenen Gantt Şeması sütunlarını ekle
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// İstenen kaynak görünümü sütunlarını ekle
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// İstenen atama görünümü sütunlarını ekle
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// kodlamayı ayarla
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Ayrıca Bakınız

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


