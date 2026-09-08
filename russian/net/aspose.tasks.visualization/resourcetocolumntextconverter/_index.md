---
title: "Делегат ResourceToColumnTextConverter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конвертер строковых данных ресурсов в столбцы"
type: docs
weight: 3340
url: /ru/net/aspose.tasks.visualization/resourcetocolumntextconverter/
---
## ResourceToColumnTextConverter delegate

Преобразователь данных ресурса в строку столбца.

```csharp
public delegate string ResourceToColumnTextConverter(Resource resource);
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ресурс | Ресурс | Текущий ресурс. |

### Возвращаемое значение

Строковые данные для столбца.

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

* class [Resource](../../aspose.tasks/resource/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


