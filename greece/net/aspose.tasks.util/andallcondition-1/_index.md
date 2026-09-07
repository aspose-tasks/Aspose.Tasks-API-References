---
title: "Κλάση AndAllConditionT"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Util.AndAllCondition1T κλάση. Εφαρμόζει λογικό AND σε όλες τις συνθήκες. Για παράδειγμα cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /el/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Εφαρμόζει λογικό AND σε όλες τις συνθήκες. Για παράδειγμα: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος του αντικειμένου στο οποίο θα εφαρμοστεί η διεπαφή μεθόδου. |

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | Αρχικοποιεί μια νέα παρουσία της κλάσης `AndAllCondition`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Επιστρέφει true εάν το καθορισμένο αντικείμενο ικανοποιεί τις συνθήκες. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε &lt;see cref="Aspose.Tasks.Util.AndAllCondition`1" /&gt; συνθήκη.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // συλλέξτε όλες τις εργασίες του έργου
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // δημιουργήστε μια συνθήκη φίλτρου που φιλτράρει τις μη-κενές εργασίες
                             new NotNullCondition(),

                             // δημιουργήστε μια συνθήκη φίλτρου που φιλτράρει τις συνοπτικές εργασίες
                             new SummaryCondition()
                         };

    // και συνδέστε τα εφαρμόζοντας τη συνθήκη <see cref="Aspose.Tasks.Util.AndAllCondition`1" />
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // εφαρμόστε τη συνθήκη στα συλλεγμένα tasks
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

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


