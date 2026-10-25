---
title: "ListUtils.Find"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ListUtils. Найти первое вхождение элемента списка, которое удовлетворяет указанному условию"
type: docs
weight: 30
url: /ru/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Найти первое вхождение элемента списка, который удовлетворяет указанному условию.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Параметр | Описание |
| --- | --- |
| T | Тип объекта для поиска. |
| list | Список для обработки. |
| cond | Условие, используемое для поиска элемента в указанном списке. |

### Возвращаемое значение

Элемент списка или null.

## Примеры

Показывает, как работать с методом Find утилиты списка.

```csharp
public void WorkWithListUtilsFind()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> taskFilters = project.TaskFilters.ToList();

    Assert.AreEqual(3, taskFilters.Count, "Project.TaskFilters count");

    var filter = ListUtils.Find(taskFilters, new FilterByName("&All Tasks"));

    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Filter Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

public class FilterByName : ICondition<Filter>
{
    private readonly string name;

    public FilterByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Возвращает true, если указанный объект удовлетворяет условиям.
    /// </summary>
    /// <param name="el">Объект для проверки.</param>
    /// <returns>True, если объект удовлетворяет условиям.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### См. также

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


