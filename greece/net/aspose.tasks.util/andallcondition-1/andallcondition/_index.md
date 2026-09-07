---
title: "AndAllCondition1.AndAllCondition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής AndAllCondition. Αρχικοποιεί μια νέα παρουσία της κλάσης AndAllCondition"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

Αρχικοποιεί μια νέα παρουσία της [`AndAllCondition`](../) κλάσης.

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| συνθήκες | List`1 | Η λίστα των συνθηκών. |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


