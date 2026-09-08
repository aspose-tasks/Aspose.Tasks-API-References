---
title: "ResourceViewColumn.ResourceViewColumn"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ResourceViewColumn. Инициализирует новый экземпляр класса ResourceViewColumn"
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/resourceviewcolumn/resourceviewcolumn/
---
## ResourceViewColumn(string, int, ResourceToColumnTextConverter, Field) {#constructor_2}

Инициализирует новый экземпляр класса [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter, 
    Field field)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | Строка | Имя столбца. |
| ширина | Int32 | Ширина столбца в пикселях. |
| конвертер | ResourceToColumnTextConverter | Конвертер данных ресурса в текст столбца. |
| поле | Поле | Поле столбца. |

## Примеры

Показывает, как добавить столбцы представления ресурсов для экспорта.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// итерация по столбцам
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### См. также

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(string, int, ResourceToColumnTextConverter) {#constructor_1}

Инициализирует новый экземпляр класса [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | Строка | Имя столбца. |
| ширина | Int32 | Ширина столбца в пикселях. |
| конвертер | ResourceToColumnTextConverter | Конвертер данных ресурса в текст столбца. |

## Примеры

Показывает, как добавить столбцы представления ресурсов для экспорта.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// итерация по столбцам
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### См. также

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(int, Field) {#constructor}

Инициализирует новый экземпляр класса [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(int width, Field field)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ширина | Int32 | Ширина столбца в пикселях. |
| поле | Поле | Поле столбца. |

## Примеры

Показывает, как добавить столбцы представления ресурсов для экспорта.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// итерация по столбцам
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### См. также

* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


