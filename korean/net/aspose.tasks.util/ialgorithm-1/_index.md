---
title: "인터페이스 IAlgorithmT"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.IAlgorithm1T 인터페이스. T 객체 목록에 적용할 수 있는 알고리즘을 나타냅니다"
type: docs
weight: 2710
url: /ko/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

*T* 객체 목록에 적용할 수 있는 알고리즘을 나타냅니다.

```csharp
public interface IAlgorithm<in T>
```

| 매개변수 | 설명 |
| --- | --- |
| T | 메서드 인터페이스를 적용할 객체 유형. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | 목록의 객체를 처리합니다. [`PreAlg`](./prealg/) 이후에 호출됩니다; |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | 객체 처리 후에 호출됩니다. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | 객체 처리 전에 호출됩니다. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


