---
title: "TaskBaselineCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskBaselineCollection मेथड। TaskBaselineCollection ऑब्जेक्ट को TaskBaseline ऑब्जेक्ट्स की सूची में बदलता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/taskbaselinecollection/tolist/
---
## TaskBaselineCollection.ToList method

TaskBaselineCollection ऑब्जेक्ट को [`TaskBaseline`](../../taskbaseline/) ऑब्जेक्ट्स की सूची में बदलता है।

```csharp
public List<TaskBaseline> ToList()
```

### रिटर्न वैल्यू

सूची [`TaskBaseline`](../../taskbaseline/) ऑब्जेक्ट्स की।

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


