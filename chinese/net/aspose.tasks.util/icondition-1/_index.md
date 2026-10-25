---
title: "接口 IConditionT"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.ICondition1T 接口。表示可被过滤器或搜索方法使用的条件"
type: docs
weight: 2720
url: /zh/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

表示可被过滤器或搜索方法使用的条件。

```csharp
public interface ICondition<in T>
```

| 参数 | 描述 |
| --- | --- |
| T | 要将方法接口应用于的对象类型。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | 如果指定的对象满足条件，则返回 true。 |

## 示例

展示如何使用列表工具的 Filter 方法。

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
    /// 如果指定的对象满足条件，则返回 true。
    /// </summary>
    /// <param name=\"el\">要检查的对象。</param>
    /// <returns>如果对象满足条件，则返回 True。</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### 另见

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


