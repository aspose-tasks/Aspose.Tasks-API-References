---
title: "Класс ResourceViewColumn"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.ResourceViewColumn. Класс представления проектов, используемый в представлениях ResourceUsage и ResourceSheet"
type: docs
weight: 3350
url: /ru/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

Класс представления проекта, используемый в представлениях ResourceUsage и ResourceSheet.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | Инициализирует новый экземпляр класса `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | Инициализирует новый экземпляр класса `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | Инициализирует новый экземпляр класса `ResourceViewColumn`. |

## Свойства

| Имя | Описание |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Поле столбца. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Получает имя столбца. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Получает или задает выравнивание текста (может быть одним из значений перечисления [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Получает или задает обратный вызов, который можно использовать для настройки внешнего вида ячеек столбца. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Получает ширину столбца. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Преобразует текущий ресурс в текст столбца. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


