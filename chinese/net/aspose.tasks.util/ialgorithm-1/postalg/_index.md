---
title: "IAlgorithm1.PostAlg"
second_title: "Aspose.Tasks for .NET API 参考"
description: "IAlgorithm 方法。对象处理后调用。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.util/ialgorithm-1/postalg/
---
## IAlgorithm&lt;T&gt;.PostAlg method

在处理对象之后调用。

```csharp
public void PostAlg(T el, int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 已处理的对象。 |
| index | Int32 | 对象的索引。 |

## 示例

展示如何使用列表工具的 Apply 方法。

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

### 另见

* interface [IAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../ialgorithm-1/)
* assembly [Aspose.Tasks](../../../)


