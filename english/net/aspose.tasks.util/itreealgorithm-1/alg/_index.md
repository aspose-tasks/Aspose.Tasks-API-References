---
title: ITreeAlgorithm1.Alg
second_title: Aspose.Tasks for .NET API Reference
description: ITreeAlgorithm method. Processes a node of a tree
type: docs
weight: 10
url: /net/aspose.tasks.util/itreealgorithm-1/alg/
---
## ITreeAlgorithm&lt;T&gt;.Alg method

Processes a node of a tree.

```csharp
public void Alg(T el, int level)
```

| Parameter | Type | Description |
| --- | --- | --- |
| el | T | Node to process. |
| level | Int32 | Tree node level. |

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.Util.ITreeAlgorithm`1" /&gt; tree based algorithm.

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

    // use tree algorithm to gather common work and update work 
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>Initializes a new instance of the <see cref="WorkAccumulator" /> class.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // there is nothing to do in pre algorithm steps
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
        // there is nothing to do in post algorithm steps
    }
}
```

### See Also

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


