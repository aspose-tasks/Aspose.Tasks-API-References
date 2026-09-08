---
title: "Class AndAllConditionT"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.AndAllCondition1T class. Past logische EN toe op alle voorwaarden. Bijvoorbeeld cond1 EN cond2 EN cond3"
type: docs
weight: 2660
url: /nl/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Past logische EN toe op alle voorwaarden. Bijvoorbeeld: cond1 EN cond2 EN cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object waarop de methodinterface moet worden toegepast. |

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | Initialiseert een nieuw exemplaar van de `AndAllCondition` klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Retourneert true als het opgegeven object aan de voorwaarden voldoet. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


