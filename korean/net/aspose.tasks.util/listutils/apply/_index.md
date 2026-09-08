---
title: "ListUtils.Apply"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ListUtils 메서드. 지정된 위치부터 각 리스트 요소에 알고리즘을 적용합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

지정된 위치부터 시작하여 각 리스트 요소에 알고리즘을 적용합니다.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| 매개변수 | 설명 |
| --- | --- |
| T | 알고리즘을 적용할 객체의 유형입니다. |
| 목록 | 처리할 리스트입니다. |
| 알고리즘 | 적용된 알고리즘. |
| 시작인덱스 | 시작 요소 위치입니다. |

## 예제

list util Apply 메서드를 사용하는 방법을 보여줍니다.

```csharp
public void WorkWithListUtilsApply()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Apply(filters, new RenameAlgorithm(), 0);

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

private class RenameAlgorithm : IAlgorithm<Filter>
{
    private int current;

    public RenameAlgorithm()
    {
        this.current = 0;
    }

    public void PreAlg(Filter el, int index)
    {
        this.current++;
    }

    public void Alg(Filter el, int index)
    {
        el.Name = el.Name + " " + this.current;
    }

    public void PostAlg(Filter el, int index)
    {
    }
}
```

### 또 보기

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


