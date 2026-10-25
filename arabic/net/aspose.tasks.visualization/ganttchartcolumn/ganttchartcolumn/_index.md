---
title: "GanttChartColumn.GanttChartColumn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ GanttChartColumn. يهيء مثيلاً جديداً من فئة GanttChartColumn."
type: docs
weight: 10
url: /ar/net/aspose.tasks.visualization/ganttchartcolumn/ganttchartcolumn/
---
## GanttChartColumn(string, int, TaskToColumnTextConverter, Field) {#constructor_3}

يُنشئ مثيلًا جديدًا من الفئة GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter, Field field)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم العمود. |
| العرض | Int32 | عرض العمود بالبكسل. |
| محول | TaskToColumnTextConverter | محول بيانات المهمة إلى نص العمود. |
| حقل | حقل | حقل العمود. |

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

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, TaskToColumnTextConverter) {#constructor_2}

يُنشئ مثيلًا جديدًا من الفئة GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم العمود. |
| العرض | Int32 | عرض العمود بالبكسل. |
| محول | TaskToColumnTextConverter | محول بيانات المهمة إلى نص العمود. |

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

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(int, Field) {#constructor}

يُنشئ مثيلًا جديدًا من الفئة GanttChartColumn.

```csharp
public GanttChartColumn(int width, Field field)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العرض | Int32 | عرض العمود بالبكسل. |
| حقل | حقل | حقل العمود. |

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

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, Field) {#constructor_1}

يُنشئ مثيلًا جديدًا من الفئة GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, Field field)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم العمود. |
| العرض | Int32 | عرض العمود بالبكسل. |
| حقل | حقل | حقل العمود. |

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

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


