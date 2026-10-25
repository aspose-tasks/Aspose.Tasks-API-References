---
title: "AndAllCondition1.AndAllCondition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "AndAllCondition 构造函数。 初始化 AndAllCondition 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

初始化 [`AndAllCondition`](../) 类的新实例。

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 条件 | List`1 | 条件列表。 |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


