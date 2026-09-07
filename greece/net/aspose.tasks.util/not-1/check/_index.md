---
title: "Not1.Check"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Not μέθοδος. Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί την προϋπόθεση"
type: docs
weight: 20
url: /el/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί την προϋπόθεση.

```csharp
public bool Check(T el)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Το αντικείμενο προς έλεγχο. |

### Τιμή Επιστροφής

Αληθές εάν το αντικείμενο ικανοποιεί την προϋπόθεση.

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

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


