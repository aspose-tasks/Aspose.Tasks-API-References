---
title: "Not1.Check"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Not-methode. Retourneert true als het opgegeven object aan de voorwaarde voldoet"
type: docs
weight: 20
url: /nl/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

Retourneert true als het opgegeven object aan de voorwaarde voldoet.

```csharp
public bool Check(T el)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Het object om te controleren. |

### Retourwaarde

True als het object aan de voorwaarde voldoet.

## Voorbeelden

Toont hoe de &lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt;-voorwaarde te gebruiken.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // verzamel alle projecttaken
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // maak een filtervoorwaarde
    var filter = new NullCondition();

    // en keer het om door de <see cref=\"Aspose.Tasks.Util.Not`1\" />-voorwaarde toe te passen
    var condition = new Not<Task>(filter);

    // pas de voorwaarde toe op de verzamelde taken
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### Zie ook

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


