---
title: "Task.Baselines"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। टास्क के बेसलाइन मानों के संग्रह को प्राप्त करता है या सेट करता है"
type: docs
weight: 130
url: /hi/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

टास्क के बेसलाइन मानों का कलेक्शन प्राप्त करता है या सेट करता है।

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## उदाहरण

टास्क के बेसलाइन को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project();

// एक बेसलाइन सेट करें
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// कार्य बेसलाइन अवधि प्रदर्शित करें
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### संबंधित देखें

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


