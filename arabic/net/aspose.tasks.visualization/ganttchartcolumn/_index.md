---
title: "الفئة GanttChartColumn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.GanttChartColumn. فئة عرض المشاريع"
type: docs
weight: 3090
url: /ar/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

فئة عرض المشروع

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | يُنشئ مثيلًا جديدًا من الفئة GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | يُنشئ مثيلًا جديدًا من الفئة GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | يُنشئ مثيلًا جديدًا من الفئة GanttChartColumn. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | يُنشئ مثيلًا جديدًا من الفئة GanttChartColumn. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | حقل العمود. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | يحصل على اسم العمود. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | يحصل أو يعيّن محاذاة النص (يمكن أن تكون أحد قيم تعداد [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | يحصل على عرض العمود. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | يحوّل المهمة الحالية إلى نص العمود. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


