---
title: "类 NotT"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.Not1T 类。对指定条件应用逻辑 NOT"
type: docs
weight: 2750
url: /zh/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

对指定的条件应用逻辑非。

```csharp
public class Not<T> : ICondition<T>
```

| 参数 | 描述 |
| --- | --- |
| T | 要将方法接口应用于的对象类型。 |

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | 初始化 `Not` 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | 如果指定的对象满足条件，则返回 true。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt; 条件。

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 收集所有项目任务
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // 创建过滤条件
    var filter = new NullCondition();

    // 并通过应用 <see cref=\"Aspose.Tasks.Util.Not`1\" /> 条件来反转它
    var condition = new Not<Task>(filter);

    // 将条件应用于收集的任务
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### 另见

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


