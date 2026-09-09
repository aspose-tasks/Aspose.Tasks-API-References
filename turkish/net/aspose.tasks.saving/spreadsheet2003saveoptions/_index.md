---
title: "Sınıf Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.Spreadsheet2003SaveOptions sınıfı. Proje sayfalarını Spreadsheet2003 formatına işlerken ek seçenekler belirtmeye olanak tanır."
type: docs
weight: 2220
url: /tr/net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

Proje sayfalarını Spreadsheet2003'e render ederken ek seçenekleri belirtmeye izin verir.

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | `Spreadsheet2003SaveOptions` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | Renderlenecek atama görünümü sütunlarının listesini alır veya ayarlar ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | Renderlenecek kaynak görünümü sütunlarının listesini alır veya ayarlar ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı şemalarında renderlanan görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | Kaydedilecek görünüm sütunlarının ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) listesini alır veya ayarlar. Ayarlanmamışsa varsayılan sütunlar kaydedilir. |

## Örnekler

Projenin Spreadsheet2003 formatına dışa aktarılması sırasında dışa aktarılacak sütunların nasıl ekleneceğini gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### Ayrıca Bakınız

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


