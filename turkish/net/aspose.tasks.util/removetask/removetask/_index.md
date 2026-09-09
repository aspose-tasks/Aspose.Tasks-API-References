---
title: "RemoveTask.RemoveTask"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "RemoveTask yapıcı. RemoveTask sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.util/removetask/removetask/
---
## RemoveTask constructor

[`RemoveTask`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public RemoveTask(Task task)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Kaldırılacak görev. |

## Örnekler

&lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt; ağaç tabanlı algoritmanın nasıl kullanılacağını gösterir.

```csharp
public void WorkWithRemoveTask()
{
    var project = new Project(DataDir + "Project1.mpp");
    var task1 = project.RootTask.Children.Add("1");
    var task2 = project.RootTask.Children.Add("2");
    var task3 = project.RootTask.Children.Add("3");
    var task4 = project.RootTask.Children.Add("4");

    List<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks before using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    Console.WriteLine();

    // Ağaç tabanlı algoritmayı kullanarak task1'i ağaçtan sil.
    var algorithm = new RemoveTask(task1);

    // Algoritmayı görev ağacına uygula.
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // Sonuçları kontrol et.
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### Ayrıca Bakınız

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


