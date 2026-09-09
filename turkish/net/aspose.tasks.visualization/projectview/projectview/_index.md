---
title: "ProjectView.ProjectView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectView yapıcı. ProjectView sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.visualization/projectview/projectview/
---
## ProjectView constructor

[`ProjectView`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ProjectView(IEnumerable<ViewColumn> columns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütunlar | IEnumerable`1 | Görünüm sütunlarının bir listesi. |

## Örnekler

Özel bir sütun kümesiyle bir görünüm kullanarak bir projenin nasıl kaydedileceğini gösterir.

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

// görünüm sütunları üzerinde yinele
foreach (var column in options.View.Columns)
{
    Console.WriteLine("Column Name: " + column.Name);
}

options.PresentationFormat = PresentationFormat.TaskUsage;
project.Save(OutDir + "TaskUsageProjectView_Columns.pdf", options);
```

### Ayrıca Bakınız

* class [ViewColumn](../../viewcolumn/)
* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


