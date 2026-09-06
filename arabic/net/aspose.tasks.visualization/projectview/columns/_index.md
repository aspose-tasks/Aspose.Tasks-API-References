---
title: "ProjectView.Columns"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectView. تسترجع أعمدة عرض المشروع"
type: docs
weight: 70
url: /ar/net/aspose.tasks.visualization/projectview/columns/
---
## ProjectView.Columns property

يحصل على أعمدة عرض المشروع.

```csharp
public List<ViewColumn> Columns { get; }
```

## الأمثلة

يوضح كيفية حفظ مشروع مع عرض يحتوي على مجموعة مخصصة من الأعمدة.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new GanttChartColumn("Name", 100, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("Finish", 100, Field.TaskFinish),
    new GanttChartColumn("Cost2", 80, Field.TaskCost2),
    new GanttChartColumn("Number6", 80, Field.TaskNumber6),
    new GanttChartColumn("Date6", 80, Field.TaskDate6),
    new GanttChartColumn("Flag6", 80, Field.TaskFlag6),
    new GanttChartColumn("Flag18", 80, Field.TaskFlag18),
    new GanttChartColumn("Duration6", 80, Field.TaskDuration6)
};
options.View = new ProjectView(columns);

// التكرار عبر أعمدة العرض
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### انظر أيضًا

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


