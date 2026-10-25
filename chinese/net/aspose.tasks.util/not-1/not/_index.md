---
title: "Not1.Not"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Not 构造函数。初始化 Not 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.util/not-1/not/
---
## Not&lt;T&gt; constructor

初始化 [`Not`](../) 类的新实例。

```csharp
public Not(ICondition<T> condition)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 条件 | ICondition`1 | 指定的条件。 |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


