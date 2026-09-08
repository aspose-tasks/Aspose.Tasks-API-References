---
title: "Klasse AndT"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.And1T-klasse. Past logische EN toe op de opgegeven voorwaarden"
type: docs
weight: 2670
url: /nl/net/aspose.tasks.util/and-1/
---
## And&lt;T&gt; class

Past logische EN toe op de opgegeven voorwaarden.

```csharp
public class And<T> : ICondition<T>
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object waarop de methodinterface moet worden toegepast. |

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [And](and/)(ICondition&lt;T&gt;, ICondition&lt;T&gt;) | Initialiseert een nieuw exemplaar van de `And`-klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Check](../../aspose.tasks.util/and-1/check/)(T) | Retourneert true als het opgegeven object aan de voorwaarden voldoet. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


