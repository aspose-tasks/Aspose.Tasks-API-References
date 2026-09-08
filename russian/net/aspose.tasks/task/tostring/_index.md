---
title: "Task.ToString"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Возвращает краткое строковое представление задачи. Точные детали представления не указаны и могут изменяться."
type: docs
weight: 1420
url: /ru/net/aspose.tasks/task/tostring/
---
## Task.ToString method

Возвращает короткое строковое представление задачи. Точные детали представления не определены и могут измениться.

```csharp
public override string ToString()
```

### Возвращаемое значение

короткая строка, представляющая объект задачи.

## Примеры

Показывает, как сортировать задачи по имени.

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

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


