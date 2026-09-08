---
title: "Класс Filter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Filter. Представляет фильтр в Project"
type: docs
weight: 600
url: /ru/net/aspose.tasks/filter/
---
## Filter class

Представляет фильтр в Project.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Filter](filter/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Получает или задает критерии, которым задачи или ресурсы должны соответствовать для отображения в представлении MSP. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Получает тип фильтра. |
| [Index](../../aspose.tasks/filter/index/) { get; } | Получает индекс объекта `Filter` в содержащем объекте Filters. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Получает или задает имя объекта Filter. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Получает или задает значение, указывающее, отображает ли проект имя фильтра в раскрывающемся списке Filter на вкладке View ленты. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Получает или задает значение, указывающее, отображаются ли связанные строки сводки для фильтра. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Получает уникальный идентификатор фильтра. |

## Методы

| Имя | Описание |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | Сравнивает этот экземпляр с указанным экземпляром класса `Filter` и возвращает указание их относительного порядка. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту AssignmentBaseline. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту AssignmentBaseline. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Возвращает значение хеш-кода для фильтра. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Возвращает значение, указывающее, больше ли этот экземпляр указанного объекта. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Возвращает значение, указывающее, больше ли или равен этот экземпляр указанному объекту. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Возвращает значение, указывающее, не равен ли этот экземпляр указанному объекту. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Возвращает значение, указывающее, меньше ли этот экземпляр указанного объекта. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Возвращает значение, указывающее, меньше ли или равен этот экземпляр указанному объекту. |

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


