---
title: "Task.ToString"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task method. एक टास्क का छोटा स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और बदल सकते हैं।"
type: docs
weight: 1420
url: /hi/net/aspose.tasks/task/tostring/
---
## Task.ToString method

एक कार्य का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और परिवर्तन के अधीन हो सकते हैं।

```csharp
public override string ToString()
```

### रिटर्न वैल्यू

छोटा स्ट्रिंग जो टास्क ऑब्जेक्ट का प्रतिनिधित्व करता है।

## उदाहरण

दिखाता है कि टास्क को नाम के अनुसार कैसे क्रमबद्ध किया जाए।

```csharp
public void SortTasksByName()
{
    var project = new Project(DataDir + "project-sort.mpp");
    var collector = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, collector, 0);
    List<Task> tasks = collector.Tasks;

    tasks.Sort(new TaskNameComparer());

    foreach (var task in tasks)
    {
        Console.WriteLine(task.ToString());
    }
}

private class TaskNameComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        if (y == null)
        {
            return 1;
        }

        if (string.IsNullOrEmpty(x.Get(Tsk.Name)))
        {
            return 1;
        }

        if (string.IsNullOrEmpty(y.Get(Tsk.Name)))
        {
            return -1;
        }

        return string.Compare(x.Get(Tsk.Name), y.Get(Tsk.Name), StringComparison.Ordinal);
    }
}
```

### संबंधित देखें

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


