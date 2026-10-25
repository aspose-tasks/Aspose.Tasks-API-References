---
title: "Интерфейс IConditionT"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Интерфейс Aspose.Tasks.Util.ICondition1T. Представляет условие, которое может использоваться фильтрами или методами поиска"
type: docs
weight: 2720
url: /ru/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Представляет условие, которое может использоваться фильтрами или методами поиска.

```csharp
public interface ICondition<in T>
```

| Параметр | Описание |
| --- | --- |
| T | Тип объекта, к которому применяется интерфейс метода. |

## Методы

| Имя | Описание |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Возвращает true, если указанный объект удовлетворяет условиям. |

## Примеры

Показывает, как работать с методом Filter утилиты списка.

```csharp
public void WorkWithListUtilsFilter()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Filter(filters, new FilterByIndex(1));

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

public class FilterByIndex : ICondition<Filter>
{
    private readonly int index;

    public FilterByIndex(int index)
    {
        this.index = index;
    }

    /// <summary>
    /// Возвращает true, если указанный объект удовлетворяет условиям.
    /// </summary>
    /// <param name="el">Объект для проверки.</param>
    /// <returns>True, если объект удовлетворяет условиям.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### См. также

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


