---
title: "TaskBaselineCollection.Count"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskBaselineCollection प्रॉपर्टी। इस TaskBaselineCollection ऑब्जेक्ट में सम्मिलित ऑब्जेक्ट्स की संख्या प्राप्त करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/taskbaselinecollection/count/
---
## TaskBaselineCollection.Count property

इस TaskBaselineCollection ऑब्जेक्ट में मौजूद ऑब्जेक्ट्स की संख्या प्राप्त करता है।

```csharp
public int Count { get; }
```

## उदाहरण

टास्क बेसलाइन संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project();

// प्रोजेक्ट बेसलाइन बनाएं
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// टास्क बेसलाइन प्रिंट करें
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// आइए सभी बेसलाइन साफ़ करें
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### संबंधित देखें

* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


