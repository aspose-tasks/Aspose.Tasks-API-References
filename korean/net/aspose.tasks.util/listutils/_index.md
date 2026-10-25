---
title: "클래스 ListUtils"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.ListUtils 클래스. 리스트 처리용 유틸리티 클래스"
type: docs
weight: 2740
url: /ko/net/aspose.tasks.util/listutils/
---
## ListUtils class

리스트 처리를 위한 유틸리티 클래스.

```csharp
public static class ListUtils
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | 지정된 위치부터 시작하여 각 리스트 요소에 알고리즘을 적용합니다. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | 지정된 조건에 따라 리스트 요소를 필터링합니다. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | 지정된 조건을 만족하는 리스트 요소의 첫 번째 발생을 찾습니다. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


