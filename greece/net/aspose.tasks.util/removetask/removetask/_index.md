---
title: "RemoveTask.RemoveTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής RemoveTask. Αρχικοποιεί μια νέα παρουσία της κλάσης RemoveTask"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/removetask/removetask/
---
## RemoveTask constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`RemoveTask`](../).

```csharp
public RemoveTask(Task task)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασία | Εργασία | Εργασία για αφαίρεση. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τον αλγόριθμο βάσει δέντρου &lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt;.

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

    // Χρησιμοποιήστε αλγόριθμο βάσει δέντρου για να διαγράψετε το task1 από το δέντρο
    var algorithm = new RemoveTask(task1);

    // Εφαρμόστε τον αλγόριθμο στο δέντρο εργασιών
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // Ελέγξτε τα αποτελέσματα
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


