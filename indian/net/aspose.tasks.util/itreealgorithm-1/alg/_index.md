---
title: "ITreeAlgorithm1.Alg"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ITreeAlgorithm मेथड। एक पेड़ के नोड को प्रोसेस करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/itreealgorithm-1/alg/
---
## ITreeAlgorithm&lt;T&gt;.Alg method

ट्री के एक नोड को प्रोसेस करता है।

```csharp
public void Alg(T el, int level)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रोसेस करने के लिए नोड। |
| स्तर | Int32 | पेड़ नोड का स्तर। |

## उदाहरण

दिखाता है कि कैसे &lt;see cref=\"Aspose.Tasks.Util.ITreeAlgorithm`1\" /&gt; पेड़-आधारित एल्गोरिद्म का उपयोग किया जाए।

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

    // सामान्य कार्य एकत्र करने और कार्य को अपडेट करने के लिए पेड़ एल्गोरिद्म का उपयोग करें 
    var acc = new WorkAccumulator();
    TaskUtils.Apply(summary, acc, 0);

    var summaryWork = acc.Work.ToDouble();
    summary.Set(Tsk.Work, project.GetWork(summaryWork));
    summary.Set(Tsk.RemainingWork, project.GetWork(summaryWork));

    // ...
}

private class WorkAccumulator : ITreeAlgorithm<Task>
{
    /// <summary>एक नया इंस्टेंस <see cref=\"WorkAccumulator\" /> क्लास का प्रारंभ करता है।</summary>
    public WorkAccumulator()
    {
        this.Work = new Duration();
    }

    public Duration Work { get; private set; }

    public void PreAlg(Task el, int level)
    {
        // पूर्व एल्गोरिद्म चरणों में करने के लिए कुछ नहीं है
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
        // पोस्ट एल्गोरिद्म चरणों में करने के लिए कुछ नहीं है
    }
}
```

### संबंधित देखें

* interface [ITreeAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../itreealgorithm-1/)
* assembly [Aspose.Tasks](../../../)


