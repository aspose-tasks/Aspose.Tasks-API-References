---
title: "IAlgorithm1.PostAlg"
second_title: "Aspose.Tasks for .NET API 참조"
description: "IAlgorithm 메서드. 객체 처리 후 호출됩니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/ialgorithm-1/postalg/
---
## IAlgorithm&lt;T&gt;.PostAlg method

객체 처리 후에 호출됩니다.

```csharp
public void PostAlg(T el, int index)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 처리된 객체. |
| 인덱스 | Int32 | 객체의 인덱스. |

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

* interface [IAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../ialgorithm-1/)
* assembly [Aspose.Tasks](../../../)


