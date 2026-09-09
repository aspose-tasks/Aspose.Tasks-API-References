---
title: "Sınıf GanttChartColumn"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.GanttChartColumn sınıfı. Projeler görünüm sınıfı"
type: docs
weight: 3090
url: /tr/net/aspose.tasks.visualization/ganttchartcolumn/
---
## GanttChartColumn class

Projenin görünüm sınıfı

```csharp
public sealed class GanttChartColumn : ViewColumn
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GanttChartColumn](ganttchartcolumn/#constructor)(int, Field) | GanttChartColumn sınıfının yeni bir örneğini başlatır. |
| [GanttChartColumn](ganttchartcolumn/#constructor_1)(string, int, Field) | GanttChartColumn sınıfının yeni bir örneğini başlatır. |
| [GanttChartColumn](ganttchartcolumn/#constructor_2)(string, int, TaskToColumnTextConverter) | GanttChartColumn sınıfının yeni bir örneğini başlatır. |
| [GanttChartColumn](ganttchartcolumn/#constructor_3)(string, int, TaskToColumnTextConverter, Field) | GanttChartColumn sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/ganttchartcolumn/field/) { get; set; } | Sütun alanı. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Sütun adını alır. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Metnin hizalamasını alır veya ayarlar ([`HorizontalStringAlignment`](../horizontalstringalignment/) enum değerlerinden biri olabilir). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Sütun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı alır veya ayarlar. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Sütun genişliğini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/ganttchartcolumn/getcolumntext/)(Task) | Geçerli görevi sütun metnine dönüştürür. |

## Örnekler

Dışa aktarılacak Gantt şeması görünüm sütunlarının nasıl ekleneceğini gösterir.

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

// sütunlar üzerinde yinele
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

### Ayrıca Bakınız

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


