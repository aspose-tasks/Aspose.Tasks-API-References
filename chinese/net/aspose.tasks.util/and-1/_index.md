---
title: "类 AndT"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.And1T 类。对指定的条件应用逻辑 AND"
type: docs
weight: 2670
url: /zh/net/aspose.tasks.util/and-1/
---
## And&lt;T&gt; class

对指定的条件应用逻辑与。

```csharp
public class And<T> : ICondition<T>
```

| 参数 | 描述 |
| --- | --- |
| T | 要将方法接口应用于的对象类型。 |

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [And](and/)(ICondition&lt;T&gt;, ICondition&lt;T&gt;) | 初始化 `And` 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Check](../../aspose.tasks.util/and-1/check/)(T) | 如果指定的对象满足条件，则返回 true。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt; 条件。

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 收集所有项目任务
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // 创建过滤汇总任务的条件
    var condition1 = new SummaryCondition();

    // 创建过滤非空任务的条件
    var condition2 = new NotNullCondition();

    // 并通过应用 <see cref=\"Aspose.Tasks.Util.And`1\" /> 条件将它们连接起来
    var joinedCondition = new And<Task>(condition1, condition2);

    // 将条件应用于收集的任务
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

        // 使用其他属性...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### 另见

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


