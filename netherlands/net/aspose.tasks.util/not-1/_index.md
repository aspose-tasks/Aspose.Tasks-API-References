---
title: "Class NotT"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.Not1T class. Past logische NOT toe op de opgegeven voorwaarde"
type: docs
weight: 2750
url: /nl/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Past logische NIET toe op de opgegeven voorwaarde.

```csharp
public class Not<T> : ICondition<T>
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object waarop de methodinterface moet worden toegepast. |

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | Initialiseert een nieuw exemplaar van de `Not`-klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Retourneert true als het opgegeven object aan de voorwaarde voldoet. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


