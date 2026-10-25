---
title: "RemoveTask.RemoveTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RemoveTask कंस्ट्रक्टर। RemoveTask क्लास का नया उदाहरण प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/removetask/removetask/
---
## RemoveTask constructor

[`RemoveTask`](../) क्लास का नया उदाहरण प्रारंभ करता है।

```csharp
public RemoveTask(Task task)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | कार्य | हटाने के लिए कार्य। |

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

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


