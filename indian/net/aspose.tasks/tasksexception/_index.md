---
title: "क्लास TasksException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TasksException क्लास। मानक आंतरिक अपवाद प्रकार को दर्शाता है।"
type: docs
weight: 2520
url: /hi/net/aspose.tasks/tasksexception/
---
## TasksException class

मानक आंतरिक अपवाद प्रकार का प्रतिनिधित्व करता है।

```csharp
public class TasksException : ApplicationException
```

## उदाहरण

टूटे हुए प्रोजेक्ट की संरचना का पता लगाने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// प्रोजेक्ट की संरचना जांचें।
// The <see cref=\"TasksException\"> will be thrown if the project structure is incorrect.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


