---
title: "AndAllCondition1.AndAllCondition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "AndAllCondition-constructeur. Initialiseert een nieuw exemplaar van de AndAllCondition-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

Initialiseert een nieuw exemplaar van de [`AndAllCondition`](../) klasse.

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| voorwaarden | List`1 | De lijst met voorwaarden. |

## Voorbeelden

Toont hoe &lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt; voorwaarde te gebruiken.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // verzamel alle projecttaken
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // maak een filtervoorwaarde die niet‑null taken filtert
                             new NotNullCondition(),

                             // maak een filtervoorwaarde die samenvattende taken filtert
                             new SummaryCondition()
                         };

    // en voeg ze samen door <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /> voorwaarde toe te passen
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // pas de voorwaarde toe op de verzamelde taken
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

        // werk met andere eigenschappen...
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

### Zie ook

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


