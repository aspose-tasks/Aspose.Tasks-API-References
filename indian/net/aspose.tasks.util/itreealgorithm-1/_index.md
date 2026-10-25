---
title: "इंटरफ़ेस ITreeAlgorithmT"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.ITreeAlgorithm1T इंटरफ़ेस। एक एल्गोरिद्म का प्रतिनिधित्व करता है जिसे वस्तुओं T के पेड़ पर लागू किया जा सकता है"
type: docs
weight: 2730
url: /hi/net/aspose.tasks.util/itreealgorithm-1/
---
## ITreeAlgorithm&lt;T&gt; interface

*T* वस्तुओं के वृक्ष पर लागू की जा सकने वाली एल्गोरिद्म का प्रतिनिधित्व करता है।

```csharp
public interface ITreeAlgorithm<in T>
```

| पैरामीटर | विवरण |
| --- | --- |
| T | विधि इंटरफ़ेस लागू करने के लिए वस्तु का प्रकार। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Alg](../../aspose.tasks.util/itreealgorithm-1/alg/)(T, int) | ट्री के एक नोड को प्रोसेस करता है। |
| [PostAlg](../../aspose.tasks.util/itreealgorithm-1/postalg/)(T, int) | ट्री के नोड के प्रोसेसिंग के बाद बुलाया जाता है। |
| [PreAlg](../../aspose.tasks.util/itreealgorithm-1/prealg/)(T, int) | ट्री के नोड के प्रोसेसिंग से पहले बुलाया जाता है। |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


