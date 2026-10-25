---
title: "ListUtils.Filter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ListUtils 메서드. 지정된 조건으로 리스트 요소를 필터링합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

지정된 조건에 따라 리스트 요소를 필터링합니다.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| 매개변수 | 설명 |
| --- | --- |
| T | 필터를 적용할 객체의 유형입니다. |
| 목록 | 처리할 리스트입니다. |
| cond | 지정된 리스트를 필터링하는 데 사용되는 조건입니다. |

### 반환 값

필터링된 리스트.

## 예제

list util Filter 메서드 사용 방법을 보여줍니다.

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
    /// 지정된 객체가 조건을 만족하면 true를 반환합니다.
    /// </summary>
    /// <param name=\"el\">확인할 객체입니다.</param>
    /// <returns>객체가 조건을 만족하면 true를 반환합니다.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### 또 보기

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


