---
title: "类 ListUtils"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.ListUtils 类。用于列表处理的实用类"
type: docs
weight: 2740
url: /zh/net/aspose.tasks.util/listutils/
---
## ListUtils class

用于列表处理的实用类。

```csharp
public static class ListUtils
```

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | 从指定位置开始，对每个列表元素应用算法。 |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | 根据指定条件过滤列表元素。 |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | 查找满足指定条件的列表元素的首次出现。 |

## 示例

展示如何使用列表实用工具的 Find 方法。

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
    /// 如果指定的对象满足条件，则返回 true。
    /// </summary>
    /// <param name=\"el\">要检查的对象。</param>
    /// <returns>如果对象满足条件，则返回 True。</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### 另见

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


