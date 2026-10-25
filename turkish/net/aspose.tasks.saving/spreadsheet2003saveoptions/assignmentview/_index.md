---
title: "Spreadsheet2003SaveOptions.AssignmentView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Spreadsheet2003SaveOptions özelliği. AssignmentViewColumn'ı render etmek için atama görünümü sütunlarının bir listesini alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/
---
## Spreadsheet2003SaveOptions.AssignmentView property

Atama görünümü sütunlarını render etmek için bir liste alır veya ayarlar ([`AssignmentViewColumn`](../../../aspose.tasks.visualization/assignmentviewcolumn/)).

```csharp
public ProjectView AssignmentView { get; set; }
```

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


