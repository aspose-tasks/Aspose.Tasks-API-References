---
title: "Перечисление ItemType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.ItemType. Указывает тип элемента."
type: docs
weight: 920
url: /ru/net/aspose.tasks/itemtype/
---
## ItemType enumeration

Указывает тип элемента.

```csharp
public enum ItemType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| TaskItem | `0` | Элемент задачи. |
| ResourceItem | `1` | Элемент ресурса. |
| OtherItem | `2` | Другой элемент. |

## Примеры

Показывает, как работать с фильтрами.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// проверьте фильтры ресурсов
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


