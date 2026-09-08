---
title: "TaskUtils.Filter"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskUtils methode. Bouwt een nieuwe boom van taken die aan de voorwaarde voldoen"
type: docs
weight: 20
url: /nl/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Bouwt een nieuwe boom van taken die aan de voorwaarde voldoen.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| root | Taak | Root van de boom. |
| cond | ICondition`1 | Toegepaste voorwaarde. |

### Retourwaarde

Root van een nieuwe boom.

## Voorbeelden

Toont hoe te werken met een voorwaarde.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // bouwt een nieuwe boom van taken die aan de voorwaarde voldoen 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

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

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Retourneert true als het opgegeven object aan de voorwaarden voldoet.
    /// </summary>
    /// <param name=\"el\">Het object om te controleren.</param>
    /// <returns>True als het object aan de voorwaarden voldoet.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### Zie ook

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


