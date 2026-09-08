---
title: "And1.And"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "And constructor. Initialiseert een nieuw exemplaar van de And-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

Initialiseert een nieuw exemplaar van de [`And`](../) klasse.

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| cond1 | ICondition`1 | Eerste voorwaarde. |
| cond2 | ICondition`1 | Tweede voorwaarde. |

## Voorbeelden

Toont hoe de &lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt;-voorwaarde te gebruiken.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // verzamel alle projecttaken
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // maak een filtervoorwaarde die samenvattende taken filtert
    var condition1 = new SummaryCondition();

    // maak een filtervoorwaarde die niet‑null taken filtert
    var condition2 = new NotNullCondition();

    // en voeg ze samen door de <see cref=\"Aspose.Tasks.Util.And`1\" />-voorwaarde toe te passen
    var joinedCondition = new And<Task>(condition1, condition2);

    // pas de voorwaarde toe op de verzamelde taken
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


