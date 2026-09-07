---
title: "TaskUtils.Find"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskUtils मेथड। एक टास्क खोजता है जो टास्कों के पेड़ में शर्त को पूरा करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

टास्क्स के ट्री में शर्त को पूरा करने वाला टास्क खोजता है।

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| root | कार्य | ट्री की रूट। |
| cond | ICondition`1 | लागू की गई शर्त। |

### रिटर्न वैल्यू

टास्क यदि टास्क मिला, अन्यथा null।

## उदाहरण

दिखाता है कि कैसे &lt;see cref=\"Aspose.Tasks.Util.TaskUtils.Find\" /&gt; मेथड का उपयोग किया जाए।

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // शर्त को पूरा करने वाली टास्क की नई ट्री बनाता है 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

    // ट्री से टास्क इकट्ठा करें
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // साधारण टास्क सूची पर इटररेट करें 
    // जिसकी अवधि 2 कार्य दिवसों से अधिक या बराबर है
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// निर्दिष्ट वस्तु शर्तों को पूरा करती है तो true लौटाता है।
    /// </summary>
    /// <param name=\"el\">जाँचने वाली वस्तु।</param>
    /// <returns>यदि वस्तु शर्तों को पूरा करती है तो True।</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### संबंधित देखें

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


