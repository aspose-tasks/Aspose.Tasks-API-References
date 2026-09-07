---
title: "TaskUtils.Find"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskUtils μέθοδος. Βρίσκει μια εργασία που ικανοποιεί την προϋπόθεση σε ένα δέντρο εργασιών"
type: docs
weight: 30
url: /el/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Βρίσκει μια εργασία που ικανοποιεί την προϋπόθεση σε ένα δέντρο εργασιών.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| root | Εργασία | Ρίζα του δέντρου. |
| cond | ICondition`1 | Εφαρμοσμένη προϋπόθεση. |

### Τιμή Επιστροφής

Task εάν βρέθηκε η εργασία, διαφορετικά null.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη μέθοδο &lt;see cref="Aspose.Tasks.Util.TaskUtils.Find" /&gt;.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // δημιουργεί νέο δέντρο εργασιών που ικανοποιούν την προϋπόθεση 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

    // συλλέξτε εργασίες από ένα δέντρο
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // διατρέξτε απλή λίστα εργασιών 
    // των οποίων οι διάρκειες είναι μεγαλύτερες ή ίσες από 2 εργάσιμες ημέρες
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Επιστρέφει true εάν το συγκεκριμένο αντικείμενο ικανοποιεί τις συνθήκες.
    /// </summary>
    /// <param name="el">Το αντικείμενο προς έλεγχο.</param>
    /// <returns>True εάν το αντικείμενο ικανοποιεί τις συνθήκες.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


