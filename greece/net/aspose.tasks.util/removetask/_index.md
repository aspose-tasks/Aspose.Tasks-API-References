---
title: "Κλάση RemoveTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Util.RemoveTask. Αφαιρεί την καθορισμένη εργασία από ένα δέντρο εργασιών"
type: docs
weight: 2760
url: /el/net/aspose.tasks.util/removetask/
---
## RemoveTask class

Αφαιρεί την καθορισμένη εργασία από ένα δέντρο εργασιών.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RemoveTask](removetask/)(Task) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `RemoveTask`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | Μην κάνετε τίποτα. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | Μην κάνετε τίποτα. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | Αφαιρεί την εργασία από την καθορισμένη γονική εργασία. |

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

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


