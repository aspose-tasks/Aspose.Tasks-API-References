---
title: "क्लास RemoveTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.RemoveTask क्लास। निर्दिष्ट कार्य को कार्यों के पेड़ से हटाता है।"
type: docs
weight: 2760
url: /hi/net/aspose.tasks.util/removetask/
---
## RemoveTask class

निर्दिष्ट कार्य को कार्यों के वृक्ष से हटाता है।

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [RemoveTask](removetask/)(Task) | `RemoveTask` क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | कुछ न करें। |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | कुछ न करें। |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | निर्दिष्ट पैरेंट टास्क से कार्य को हटाता है। |

## उदाहरण

दिखाता है कि &lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt; ट्री-आधारित एल्गोरिदम का उपयोग कैसे करें।

```csharp
public void WorkWithRemoveTask()
{
    var project = new Project(DataDir + "Project1.mpp");
    var task1 = project.RootTask.Children.Add("1");
    var task2 = project.RootTask.Children.Add("2");
    var task3 = project.RootTask.Children.Add("3");
    var task4 = project.RootTask.Children.Add("4");

    List<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks before using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    Console.WriteLine();

    // ट्री से task1 को हटाने के लिए ट्री-आधारित एल्गोरिदम का उपयोग करें
    var algorithm = new RemoveTask(task1);

    // एल्गोरिदम को टास्क ट्री पर लागू करें
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // परिणामों की जाँच करें
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### संबंधित देखें

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


