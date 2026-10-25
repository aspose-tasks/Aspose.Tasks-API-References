---
title: "TaskUtils.Filter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskUtils मेथड। ऐसी टास्क की नई ट्री बनाता है जो शर्त को पूरा करती है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

शर्त को पूरा करने वाले टास्क्स का नया ट्री बनाता है।

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| root | कार्य | ट्री की रूट। |
| cond | ICondition`1 | लागू की गई शर्त। |

### रिटर्न वैल्यू

नई ट्री की रूट।

## उदाहरण

शर्त के साथ काम करने का तरीका दिखाता है।

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // शर्त को पूरा करने वाली टास्क की नई ट्री बनाता है 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

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

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// निर्दिष्ट वस्तु शर्तों को पूरा करती है तो true लौटाता है।
    /// </summary>
    /// <param name=\"el\">जाँचने वाली वस्तु।</param>
    /// <returns>यदि वस्तु शर्तों को पूरा करती है तो True।</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### संबंधित देखें

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


