---
title: "Task.ToString"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 작업의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다."
type: docs
weight: 1420
url: /ko/net/aspose.tasks/task/tostring/
---
## Task.ToString method

작업의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다.

```csharp
public override string ToString()
```

### 반환 값

작업 객체를 나타내는 짧은 문자열.

## 예제

이름별로 작업을 정렬하는 방법을 보여줍니다.

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

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


