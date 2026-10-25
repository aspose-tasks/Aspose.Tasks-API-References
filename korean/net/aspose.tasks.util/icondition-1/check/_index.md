---
title: "ICondition1.Check"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ICondition 메서드. 지정된 객체가 조건을 만족하면 true를 반환합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

지정된 객체가 조건을 만족하면 true를 반환합니다.

```csharp
public bool Check(T el)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 검사할 객체. |

### 반환 값

객체가 조건을 만족하면 true.

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


