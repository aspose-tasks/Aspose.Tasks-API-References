---
title: "SaveOptions.View"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد قائمة بأعمدة العرض للتصوير (GanttChartColumn). إذا لم يتم تعيينها، يتم تصوير معرفات المهام وأسماء المهام وتواريخ البدء والانتهاء فقط. إذا تم تعيين كل من خصائص View و ViewSettings، فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings."
type: docs
weight: 230
url: /ar/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

يحصل أو يحدد قائمة بأعمدة العرض للتصوير ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)). إذا لم يتم تعيينها، يتم تصوير معرفات المهام، أسماء المهام، تاريخ البدء والانتهاء فقط. إذا تم تعيين كل من View و [`ViewSettings`](../viewsettings/) فإن الأعمدة من View تتجاوز الأعمدة من ViewSettings.

```csharp
public ProjectView View { get; set; }
```

## الأمثلة

يوضح كيفية إضافة أعمدة العرض لتصديرها أثناء تصدير المشروع.

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
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


