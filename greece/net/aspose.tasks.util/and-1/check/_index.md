---
title: "And1.Check"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος And. Επιστρέφει αληθές εάν το καθορισμένο αντικείμενο ικανοποιεί τις προϋποθέσεις"
type: docs
weight: 20
url: /el/net/aspose.tasks.util/and-1/check/
---
## And&lt;T&gt;.Check method

Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τις συνθήκες.

```csharp
public bool Check(T el)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Το αντικείμενο προς έλεγχο. |

### Τιμή Επιστροφής

Αληθές εάν το αντικείμενο ικανοποιεί τις προϋποθέσεις.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη συνθήκη &lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt;.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // συλλέξτε όλες τις εργασίες του έργου
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // δημιουργήστε μια συνθήκη φίλτρου που φιλτράρει τις συνοπτικές εργασίες
    var condition1 = new SummaryCondition();

    // δημιουργήστε μια συνθήκη φίλτρου που φιλτράρει τις μη-κενές εργασίες
    var condition2 = new NotNullCondition();

    // και συνδέστε τα εφαρμόζοντας τη συνθήκη <see cref=\"Aspose.Tasks.Util.And`1\" />
    var joinedCondition = new And<Task>(condition1, condition2);

    // εφαρμόστε τη συνθήκη στα συλλεγμένα tasks
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### Δείτε επίσης

* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


