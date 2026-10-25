---
title: "SaveOptions.View"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Render edilecek view sütunlarının listesini (GanttChartColumn) alır veya ayarlar. Ayarlanmamışsa yalnızca görev kimlikleri, görev adları, başlangıç ve bitiş render edilir. Hem View hem de ViewSettings özellikleri ayarlanmışsa, View'tan gelen sütunlar ViewSettings'ten gelen sütunların üzerine yazar."
type: docs
weight: 230
url: /tr/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

Render edilecek view sütunlarının listesini ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) alır veya ayarlar. Ayarlanmamışsa yalnızca görev kimlikleri, görev adları, başlangıç ve bitiş render edilir. Hem View hem de [`ViewSettings`](../viewsettings/) özellikleri ayarlanmışsa, View'tan gelen sütunlar ViewSettings'ten gelen sütunların üzerine yazar.

```csharp
public ProjectView View { get; set; }
```

## Örnekler

Projeyi dışa aktarırken export edilecek view sütunlarının nasıl ekleneceğini gösterir.

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
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


