---
title: "TaskBaselineCollection.GetEnumerator"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskBaselineCollection मेथड। इस संग्रह के लिए एक इनेमरेटर लौटाता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/taskbaselinecollection/getenumerator/
---
## TaskBaselineCollection.GetEnumerator method

इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

```csharp
public IEnumerator<TaskBaseline> GetEnumerator()
```

### रिटर्न वैल्यू

इस संग्रह के लिए एक एनेमरेटर।

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


