---
title: "FilterCollection.CopyTo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод FilterCollection. Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива"
type: docs
weight: 60
url: /ru/net/aspose.tasks/filtercollection/copyto/
---
## FilterCollection.CopyTo method

Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива.

```csharp
public void CopyTo(Filter[] array, int arrayIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| массив | Filter[] | указанный одномерный массив, в который копировать элементы |
| arrayIndex | Int32 | нуль‑базовый индекс указанного массива, с которого начинается копирование. |

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

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


