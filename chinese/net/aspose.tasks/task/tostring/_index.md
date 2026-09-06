---
title: "Task.ToString"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。返回任务的简短字符串表示。表示的具体细节未指定，可能会更改"
type: docs
weight: 1420
url: /zh/net/aspose.tasks/task/tostring/
---
## Task.ToString method

返回任务的简短字符串表示。表示的具体细节未指定，可能会更改。

```csharp
public override string ToString()
```

### 返回值

表示任务对象的简短字符串。

## 示例

展示如何按名称对任务进行排序。

```csharp
public void SortTasksByName()
{
    var project = new Project(DataDir + "project-sort.mpp");
    var collector = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, collector, 0);
    List<Task> tasks = collector.Tasks;

    tasks.Sort(new TaskNameComparer());

    foreach (var task in tasks)
    {
        Console.WriteLine(task.ToString());
    }
}

private class TaskNameComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        if (y == null)
        {
            return 1;
        }

        if (string.IsNullOrEmpty(x.Get(Tsk.Name)))
        {
            return 1;
        }

        if (string.IsNullOrEmpty(y.Get(Tsk.Name)))
        {
            return -1;
        }

        return string.Compare(x.Get(Tsk.Name), y.Get(Tsk.Name), StringComparison.Ordinal);
    }
}
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


