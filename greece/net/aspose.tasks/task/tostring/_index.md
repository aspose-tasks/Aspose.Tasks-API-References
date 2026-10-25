---
title: "Task.ToString"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς ενός task. Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν"
type: docs
weight: 1420
url: /el/net/aspose.tasks/task/tostring/
---
## Task.ToString method

Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς μιας εργασίας. Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν.

```csharp
public override string ToString()
```

### Τιμή Επιστροφής

σύντομη συμβολοσειρά που αντιπροσωπεύει το αντικείμενο task.

## Παραδείγματα

Δείχνει πώς να ταξινομήσετε τα tasks κατά όνομα.

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

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


