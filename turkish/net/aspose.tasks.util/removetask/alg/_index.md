---
title: "RemoveTask.Alg"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "RemoveTask yöntemi. Hiçbir şey yapma"
type: docs
weight: 20
url: /tr/net/aspose.tasks.util/removetask/alg/
---
## RemoveTask.Alg method

Hiçbir şey yapma.

```csharp
public void Alg(Task el, int level)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | Görev | İşlenecek nesne. |
| seviye | Int32 | Ağaç düğüm seviyesi. |

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


