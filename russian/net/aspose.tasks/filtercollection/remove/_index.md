---
title: "FilterCollection.Remove"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод FilterCollection. Удаляет первое вхождение конкретного объекта из этой коллекции"
type: docs
weight: 80
url: /ru/net/aspose.tasks/filtercollection/remove/
---
## FilterCollection.Remove method

Удаляет первое вхождение конкретного объекта из этой коллекции.

```csharp
public bool Remove(Filter item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | Filter | указанный объект для удаления. |

### Возвращаемое значение

true, если указанный объект был успешно удалён из этой коллекции; иначе false.

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


