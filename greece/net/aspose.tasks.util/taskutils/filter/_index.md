---
title: "TaskUtils.Filter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος TaskUtils. Δημιουργεί νέο δέντρο εργασιών που ικανοποιούν την προϋπόθεση"
type: docs
weight: 20
url: /el/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Δημιουργεί νέο δέντρο εργασιών που ικανοποιούν την προϋπόθεση.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| root | Εργασία | Ρίζα του δέντρου. |
| cond | ICondition`1 | Εφαρμοσμένη προϋπόθεση. |

### Τιμή Επιστροφής

Ρίζα ενός νέου δέντρου.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με μια προϋπόθεση.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // δημιουργεί νέο δέντρο εργασιών που ικανοποιούν την προϋπόθεση 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

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

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Επιστρέφει true εάν το συγκεκριμένο αντικείμενο ικανοποιεί τις συνθήκες.
    /// </summary>
    /// <param name="el">Το αντικείμενο προς έλεγχο.</param>
    /// <returns>True εάν το αντικείμενο ικανοποιεί τις συνθήκες.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


