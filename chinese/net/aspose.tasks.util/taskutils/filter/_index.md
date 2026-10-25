---
title: "TaskUtils.Filter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskUtils 方法。构建满足条件的任务新树。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

构建满足条件的任务新树。

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 根 | 任务 | 树的根。 |
| 条件 | ICondition`1 | 已应用的条件。 |

### 返回值

新树的根。

## 示例

展示如何使用条件。

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 构建满足条件的任务新树 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

    // 从树中收集任务
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // 遍历普通任务列表 
    // 其持续时间大于或等于 2 个工作日
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// 如果指定的对象满足条件，则返回 true。
    /// </summary>
    /// <param name=\"el\">要检查的对象。</param>
    /// <returns>如果对象满足条件，则返回 True。</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### 另见

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


