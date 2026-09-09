---
title: "XlsxOptions.AssignmentView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "XlsxOptions özelliği. AssignmentViewColumn'ı oluşturmak için atama görünümü sütunlarının bir listesini alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/xlsxoptions/assignmentview/
---
## XlsxOptions.AssignmentView property

Atama görünümü sütunlarını render etmek için bir liste alır veya ayarlar ([`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)).

```csharp
public ProjectView AssignmentView { get; set; }
```

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


