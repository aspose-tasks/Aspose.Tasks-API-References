---
title: "क्लास TasksReadingException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TasksReadingException क्लास। मानक आंतरिक रीडिंग अपवाद प्रकार का प्रतिनिधित्व करता है"
type: docs
weight: 2540
url: /hi/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

मानक आंतरिक पढ़ने के अपवाद प्रकार का प्रतिनिधित्व करता है।

```csharp
public class TasksReadingException : TasksLoggedException
```

## गुण

| नाम | विवरण |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | अपवाद लॉगिंग जानकारी प्राप्त करता है। |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | अपवाद ऑपरेशन जानकारी प्राप्त करता है। |

## उदाहरण

प्रोजेक्ट की रीडिंग/राइटिंग अपवादों को कैसे संभालें दिखाता है।

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### संबंधित देखें

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


