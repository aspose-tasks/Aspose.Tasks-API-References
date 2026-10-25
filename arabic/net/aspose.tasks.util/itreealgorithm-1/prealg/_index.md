---
title: "ITreeAlgorithm1.PreAlg"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ITreeAlgorithm. يتم استدعاؤها قبل معالجة عقدة من شجرة"
type: docs
weight: 30
url: /ar/net/aspose.tasks.util/itreealgorithm-1/prealg/
---
## ITreeAlgorithm&lt;T&gt;.PreAlg method

يُستدعى قبل معالجة عقدة في شجرة.

```csharp
public void PreAlg(T el, int level)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| el | T | العقدة للمعالجة. |
| المستوى | Int32 | مستوى عقدة الشجرة. |

## الأمثلة

يوضح كيفية استخدام &lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt; الخوارزمية القائمة على الشجرة.

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

    // استخدم خوارزمية الشجرة لجمع العمل المشترك وتحديث العمل
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>يُنشئ مثلاً جديداً من الفئة <see cref=\"WorkAccumulator\" />.</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // ليس هناك ما يُنفّذ في خطوات ما قبل الخوارزمية
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
        // ليس هناك ما يُنفّذ في خطوات ما بعد الخوارزمية
    }
}
```

### انظر أيضًا

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


