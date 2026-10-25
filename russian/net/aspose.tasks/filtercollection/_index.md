---
title: "Класс FilterCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.FilterCollection. Содержит список объектов Filter. Реализует интерфейс ICollectionFilter."
type: docs
weight: 610
url: /ru/net/aspose.tasks/filtercollection/
---
## FilterCollection class

Содержит список объектов [`Filter`](../filter/) . Реализует интерфейс ICollection&lt;Filter&gt;.

```csharp
public class FilterCollection : ICollection<Filter>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | Преобразует коллекцию фильтров в список объектов [`Filter`](../filter/). |

## Примеры

Показывает, как работать с коллекциями фильтров.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// перебрать фильтры задач
Console.WriteLine("Print task filters of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Filters Count: " + project.TaskFilters.Count);
foreach (var filter in project.TaskFilters)
{
    Console.WriteLine("All Tasks: " + filter.Name);
    Console.WriteLine("Task Item: " + filter.FilterType);
    Console.WriteLine("Task Filters Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Task filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
    Console.WriteLine();
}

// перебрать фильтры ресурсов
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// очистить фильтры другого проекта
otherProject.TaskFilters.Clear();

// скопировать фильтры в другой проект
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// добавить пользовательский фильтр задач
var customFilter = new Filter();
customFilter.Name = "Custom Filter";
customFilter.ShowInMenu = true;
customFilter.ShowRelatedSummaryRows = true;

if (!otherProject.TaskFilters.Contains(customFilter))
{
    if (!otherProject.TaskFilters.IsReadOnly)
    {
        otherProject.TaskFilters.Add(customFilter);
    }
}

// удалить все фильтры
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### См. также

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


