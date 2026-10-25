---
title: "Κλάση NotT"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Util.Not1T. Εφαρμόζει λογικό NOT στην καθορισμένη προϋπόθεση."
type: docs
weight: 2750
url: /el/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Εφαρμόζει λογικό NOT στην καθορισμένη συνθήκη.

```csharp
public class Not<T> : ICondition<T>
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου. |

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Not`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί την προϋπόθεση. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη συνθήκη &lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt;.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // συλλέξτε όλες τις εργασίες του έργου
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // δημιουργήστε μια συνθήκη φίλτρου
    var filter = new NullCondition();

    // και αντιστρέψτε την εφαρμόζοντας τη συνθήκη <see cref=\"Aspose.Tasks.Util.Not`1\" />
    var condition = new Not<Task>(filter);

    // εφαρμόστε τη συνθήκη στα συλλεγμένα tasks
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

        // εργαστείτε με άλλες ιδιότητες...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### Δείτε επίσης

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


