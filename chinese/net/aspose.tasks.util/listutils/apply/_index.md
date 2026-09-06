---
title: "ListUtils.Apply"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ListUtils 方法。从指定位置开始对每个列表元素应用算法"
type: docs
weight: 10
url: /zh/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

从指定位置开始，对每个列表元素应用算法。

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| 参数 | 描述 |
| --- | --- |
| T | 要对其应用算法的对象类型。 |
| 列表 | 要处理的列表。 |
| 算法 | 已应用的算法。 |
| startIndex | 起始元素位置。 |

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

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


