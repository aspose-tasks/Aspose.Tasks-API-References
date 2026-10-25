---
title: "Spreadsheet2003SaveOptions.ResourceView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Spreadsheet2003SaveOptions özelliği. Kaynak görünüm sütunlarını render etmek için bir liste alır veya ayarlar ResourceViewColumn"
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/
---
## Spreadsheet2003SaveOptions.ResourceView property

Kaynak görünüm sütunlarını render etmek için bir liste alır veya ayarlar ([`ResourceViewColumn`](../../../aspose.tasks.visualization/resourceviewcolumn/)).

```csharp
public ProjectView ResourceView { get; set; }
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


