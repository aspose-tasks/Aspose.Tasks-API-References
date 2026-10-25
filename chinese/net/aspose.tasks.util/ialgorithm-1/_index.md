---
title: "接口 IAlgorithmT"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.IAlgorithm1T 接口。表示一种可以应用于对象列表 T 的算法"
type: docs
weight: 2710
url: /zh/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

表示可应用于对象列表 *T* 的算法。

```csharp
public interface IAlgorithm<in T>
```

| 参数 | 描述 |
| --- | --- |
| T | 要将方法接口应用于的对象类型。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | 处理列表中的对象。调用于[`PreAlg`](./prealg/)之后； |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | 在处理对象之后调用。 |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | 在处理对象之前调用。 |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


