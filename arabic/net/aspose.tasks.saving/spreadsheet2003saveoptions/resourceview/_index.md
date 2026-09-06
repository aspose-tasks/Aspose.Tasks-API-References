---
title: "Spreadsheet2003SaveOptions.ResourceView"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Spreadsheet2003SaveOptions. تحصل أو تعين قائمة بأعمدة عرض الموارد لتصوير ResourceViewColumn"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/
---
## Spreadsheet2003SaveOptions.ResourceView property

تحصل أو تعين قائمة بأعمدة عرض الموارد لتصوير ([`ResourceViewColumn`](../../../aspose.tasks.visualization/resourceviewcolumn/)).

```csharp
public ProjectView ResourceView { get; set; }
```

## الأمثلة

يعرض كيفية إضافة أعمدة لتصديرها أثناء تصدير المشروع إلى تنسيق Spreadsheet2003.

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

### انظر أيضًا

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


