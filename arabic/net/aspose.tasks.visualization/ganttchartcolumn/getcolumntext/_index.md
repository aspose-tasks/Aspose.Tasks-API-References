---
title: "GanttChartColumn.GetColumnText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة GanttChartColumn. تحول المهمة الحالية إلى نص العمود."
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/ganttchartcolumn/getcolumntext/
---
## GanttChartColumn.GetColumnText method

يحوّل المهمة الحالية إلى نص العمود.

```csharp
public string GetColumnText(Task task)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | المهمة الحالية. |

### قيمة الإرجاع

نص العمود.

## الأمثلة

يوضح كيفية إضافة أعمدة عرض مخطط جانت لتصديرها.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var task = project.RootTask.Children.GetById(1);

var columns = new List<ViewColumn>
{
    new GanttChartColumn(20, Field.TaskUniqueID),
    new GanttChartColumn("Name", 150, Field.TaskName),
    new GanttChartColumn("Start", 100, Field.TaskStart),
    new GanttChartColumn("End", 100, Field.TaskFinish),
    new GanttChartColumn("R-Initials", 100, Field.TaskResourceInitials),
    new GanttChartColumn("R-Names", 100, Field.TaskResourceNames),
    new GanttChartColumn("Work", 50, Field.TaskWork),
    new GanttChartColumn(
        "Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new GanttChartColumn(
        "Actual Cost", 
        80,
        delegate(Task t)
        {
            return t.Get(Tsk.ActualCost).ToString(CultureInfo.InvariantCulture);
        },
        Field.TaskActualCost)
};

// التكرار عبر الأعمدة
foreach (var column in columns)
{
    var col = (GanttChartColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(task));
    Console.WriteLine();
}

var options = new CsvOptions
{
    View = new ProjectView(columns)
};

project.Save(OutDir + "WorkWithGanttChartColumn_out.csv", options);
```

### انظر أيضًا

* class [Task](../../../aspose.tasks/task/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


