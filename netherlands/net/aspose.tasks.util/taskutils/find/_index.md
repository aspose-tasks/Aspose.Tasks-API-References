---
title: "TaskUtils.Find"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskUtils-methode. Vindt een taak die voldoet aan de voorwaarde in een boom van taken"
type: docs
weight: 30
url: /nl/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Vindt een taak die aan de voorwaarde voldoet in een boom van taken.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| root | Taak | Root van de boom. |
| cond | ICondition`1 | Toegepaste voorwaarde. |

### Retourwaarde

Taak als de taak werd gevonden, anders null.

## Voorbeelden

Toont hoe de &lt;see cref="Aspose.Tasks.Util.TaskUtils.Find" /&gt; methode te gebruiken.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // bouwt een nieuwe boom van taken die aan de voorwaarde voldoen 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

    // verzamel taken uit een boom
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // itereren over een eenvoudige lijst van taken 
    // waarvan de duur groter of gelijk is aan 2 werkdagen
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Retourneert true als het opgegeven object aan de voorwaarden voldoet.
    /// </summary>
    /// <param name=\"el\">Het object om te controleren.</param>
    /// <returns>True als het object aan de voorwaarden voldoet.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### Zie ook

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


