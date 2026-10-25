---
title: "Κλάση AndT"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Util.And1T κλάση. Εφαρμόζει λογικό AND στις καθορισμένες συνθήκες"
type: docs
weight: 2670
url: /el/net/aspose.tasks.util/and-1/
---
## And&lt;T&gt; class

Εφαρμόζει λογικό AND στις καθορισμένες συνθήκες.

```csharp
public class And<T> : ICondition<T>
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου. |

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [And](and/)(ICondition&lt;T&gt;, ICondition&lt;T&gt;) | Αρχικοποιεί μια νέα παρουσία της κλάσης `And`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Check](../../aspose.tasks.util/and-1/check/)(T) | Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τις συνθήκες. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


