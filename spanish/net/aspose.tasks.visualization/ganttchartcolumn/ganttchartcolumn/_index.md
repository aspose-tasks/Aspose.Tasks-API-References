---
title: "GanttChartColumn.GanttChartColumn"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de GanttChartColumn. Inicializa una nueva instancia de la clase GanttChartColumn"
type: docs
weight: 10
url: /es/net/aspose.tasks.visualization/ganttchartcolumn/ganttchartcolumn/
---
## GanttChartColumn(string, int, TaskToColumnTextConverter, Field) {#constructor_3}

Inicializa una nueva instancia de la clase GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter, Field field)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | Nombre de la columna. |
| ancho | Int32 | Ancho de la columna en píxeles. |
| convertidor | TaskToColumnTextConverter | Convertidor de datos de tarea a texto de columna. |
| campo | Campo | Campo de columna. |

## Ejemplos

Muestra cómo agregar columnas de vista de diagrama de Gantt para exportar.

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

// iterar sobre columnas
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

### Ver también

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, TaskToColumnTextConverter) {#constructor_2}

Inicializa una nueva instancia de la clase GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, TaskToColumnTextConverter converter)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | Nombre de la columna. |
| ancho | Int32 | Ancho de la columna en píxeles. |
| convertidor | TaskToColumnTextConverter | Convertidor de datos de tarea a texto de columna. |

## Ejemplos

Muestra cómo agregar columnas de vista de diagrama de Gantt para exportar.

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

// iterar sobre columnas
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

### Ver también

* delegate [TaskToColumnTextConverter](../../tasktocolumntextconverter/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(int, Field) {#constructor}

Inicializa una nueva instancia de la clase GanttChartColumn.

```csharp
public GanttChartColumn(int width, Field field)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ancho | Int32 | Ancho de columna en píxeles. |
| campo | Campo | Campo de columna. |

## Ejemplos

Muestra cómo agregar columnas de vista de diagrama de Gantt para exportar.

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

// iterar sobre columnas
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

### Ver también

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## GanttChartColumn(string, int, Field) {#constructor_1}

Inicializa una nueva instancia de la clase GanttChartColumn.

```csharp
public GanttChartColumn(string name, int width, Field field)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | Nombre de la columna. |
| ancho | Int32 | Ancho de columna en píxeles. |
| campo | Campo | Campo de columna. |

## Ejemplos

Muestra cómo agregar columnas de vista de diagrama de Gantt para exportar.

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

// iterar sobre columnas
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

### Ver también

* enum [Field](../../../aspose.tasks/field/)
* class [GanttChartColumn](../)
* namespace [Aspose.Tasks.Visualization](../../ganttchartcolumn/)
* assembly [Aspose.Tasks](../../../)


