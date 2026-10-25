---
title: "인터페이스 IConditionT"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.ICondition1T 인터페이스. 필터 또는 검색 메서드에서 사용할 수 있는 조건을 나타냅니다."
type: docs
weight: 2720
url: /ko/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

필터 또는 검색 메서드에서 사용할 수 있는 조건을 나타냅니다.

```csharp
public interface ICondition<in T>
```

| 매개변수 | 설명 |
| --- | --- |
| T | 메서드 인터페이스를 적용할 객체 유형. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | 지정된 객체가 조건을 만족하면 true를 반환합니다. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


