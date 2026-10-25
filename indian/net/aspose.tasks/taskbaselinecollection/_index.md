---
title: "क्लास TaskBaselineCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskBaselineCollection क्लास। TaskBaseline ऑब्जेक्ट्स का संग्रह दर्शाता है।"
type: docs
weight: 2380
url: /hi/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

[`TaskBaseline`](../taskbaseline/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | इस TaskBaselineCollection ऑब्जेक्ट में मौजूद ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकती है। |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | इस संग्रह से बेसलाइन को हटाता है। |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | TaskBaselineCollection ऑब्जेक्ट को [`TaskBaseline`](../taskbaseline/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

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

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


