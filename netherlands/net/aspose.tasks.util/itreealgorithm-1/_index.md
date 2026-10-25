---
title: "Interface ITreeAlgorithmT"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.ITreeAlgorithm1T interface. Vertegenwoordigt een algoritme dat kan worden toegepast op een boom van objecten T"
type: docs
weight: 2730
url: /nl/net/aspose.tasks.util/itreealgorithm-1/
---
## ITreeAlgorithm&lt;T&gt; interface

Stelt een algoritme voor dat kan worden toegepast op een boom van objecten *T*.

```csharp
public interface ITreeAlgorithm<in T>
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type object waarop de methodinterface moet worden toegepast. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Alg](../../aspose.tasks.util/itreealgorithm-1/alg/)(T, int) | Verwerkt een knoop van een boom. |
| [PostAlg](../../aspose.tasks.util/itreealgorithm-1/postalg/)(T, int) | Aangeroepen na verwerking van een knoop van een boom. |
| [PreAlg](../../aspose.tasks.util/itreealgorithm-1/prealg/)(T, int) | Aangeroepen vóór verwerking van een knoop van een boom. |

## Voorbeelden

Toont hoe &lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt; boomgebaseerd algoritme te gebruiken.

```csharp
public void WorkWithITreeAlgorithm()
{
    var project = new Project(DataDir + "Project1.mpp");

    var root = project.RootTask.Children.Add("Project Management");
    var summary = root.Children.Add("Manage iteration");

    var task = summary.Children.Add("Acquire staff");
    task.Set(Tsk.Start, new DateTime(1999, 5, 3, 9, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(8 * 14, TimeUnitType.Hour));
    task.Set(Tsk.Finish, project.Get(Prj.Calendar).GetFinishDateByStartAndWork(task.Get(Tsk.Start), task.Get(Tsk.Duration)));

    var resource = project.Resources.Add("Project Manager");
    resource.Set(Rsc.Type, ResourceType.Work);

    project.ResourceAssignments.Add(task, resource);

    // gebruik boomalgoritme om gemeenschappelijk werk te verzamelen en werk bij te werken 
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>Initialiseert een nieuw exemplaar van de <see cref=\"WorkAccumulator\" /> klasse.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // er is niets te doen in de pre-algoritmestappen
    }

    public void Alg(Task el, int level)
    {
        if (!el.Get(Tsk.IsSummary))
        {
            this.Work.Add(el.Get(Tsk.Work));
        }
    }

    public void PostAlg(Task el, int level)
    {
        // er is niets te doen in de post-algoritmestappen
    }
}
```

### Zie ook

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


