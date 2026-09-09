---
title: "Task.ToString"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Bir görevin kısa dize temsili döndürür. Temsilin kesin ayrıntıları belirtilmemiştir ve değişikliğe açıktır"
type: docs
weight: 1420
url: /tr/net/aspose.tasks/task/tostring/
---
## Task.ToString method

Bir görevin kısa dize temsilini döndürür. Temsilin kesin ayrıntıları belirtilmemiştir ve değişikliğe açıktır.

```csharp
public override string ToString()
```

### Dönüş Değeri

görev nesnesini temsil eden kısa dize.

## Örnekler

Görevleri ada göre nasıl sıralayacağınızı gösterir.

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

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


