---
title: "ListUtils.Filter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ListUtils. Фильтровать элементы списка по указанному условию"
type: docs
weight: 20
url: /ru/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Отфильтровать элементы списка по указанному условию.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Параметр | Описание |
| --- | --- |
| T | Тип объекта, к которому применяется фильтр. |
| list | Список для обработки. |
| cond | Условие, используемое для фильтрации указанного списка. |

### Возвращаемое значение

Отфильтрованный список.

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


