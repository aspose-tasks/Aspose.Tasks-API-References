---
title: "ListUtils.Find"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ListUtils 메서드. 지정된 조건을 만족하는 리스트 요소의 첫 번째 발생을 찾습니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

지정된 조건을 만족하는 리스트 요소의 첫 번째 발생을 찾습니다.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| 매개변수 | 설명 |
| --- | --- |
| T | 찾을 객체의 유형입니다. |
| 목록 | 처리할 리스트입니다. |
| cond | 지정된 리스트에서 요소를 찾는 데 사용되는 조건입니다. |

### 반환 값

리스트 요소 또는 null입니다.

## 예제

list util Find 메서드 사용 방법을 보여줍니다.

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
    /// 지정된 객체가 조건을 만족하면 true를 반환합니다.
    /// </summary>
    /// <param name=\"el\">확인할 객체입니다.</param>
    /// <returns>객체가 조건을 만족하면 true를 반환합니다.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### 또 보기

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


