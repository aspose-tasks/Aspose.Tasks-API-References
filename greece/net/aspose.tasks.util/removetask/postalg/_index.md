---
title: "RemoveTask.PostAlg"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "RemoveTask μέθοδος. Δεν κάνει τίποτα"
type: docs
weight: 30
url: /el/net/aspose.tasks.util/removetask/postalg/
---
## RemoveTask.PostAlg method

Μην κάνετε τίποτα.

```csharp
public void PostAlg(Task el, int level)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | Εργασία | Αντικείμενο προς επεξεργασία. |
| επίπεδο | Int32 | Επίπεδο κόμβου δέντρου. |

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


