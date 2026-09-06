---
title: "ListUtils.Find"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ListUtils 方法。查找满足指定条件的列表元素的第一次出现"
type: docs
weight: 30
url: /zh/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

查找满足指定条件的列表元素的首次出现。

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| 参数 | 描述 |
| --- | --- |
| T | 要查找的对象类型。 |
| 列表 | 要处理的列表。 |
| 条件 | 用于在指定列表中查找元素的条件。 |

### 返回值

列表元素或 null。

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


