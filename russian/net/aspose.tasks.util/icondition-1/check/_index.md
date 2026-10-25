---
title: "ICondition1.Check"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ICondition. Возвращает true, если указанный объект удовлетворяет условиям"
type: docs
weight: 10
url: /ru/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

Возвращает true, если указанный объект удовлетворяет условиям.

```csharp
public bool Check(T el)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| el | T | Объект для проверки. |

### Возвращаемое значение

True, если объект удовлетворяет условиям.

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


