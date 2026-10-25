---
title: "类 AndAllConditionT"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Util.AndAllCondition1T 类。对所有条件应用逻辑 AND。例如 cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /zh/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

对所有条件应用逻辑与。例如：cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| 参数 | 描述 |
| --- | --- |
| T | 要将方法接口应用于的对象类型。 |

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | 初始化 `AndAllCondition` 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | 如果指定的对象满足条件，则返回 true。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt; 条件。

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 收集所有项目任务
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // 创建过滤非空任务的条件
                             new NotNullCondition(),

                             // 创建过滤汇总任务的条件
                             new SummaryCondition()
                         };

    // 并通过应用 <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /> 条件将它们连接起来
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // 将条件应用于收集的任务
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

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


