---
title: "क्लास TasksLoggedException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TasksLoggedException क्लास। मानक आंतरिक अपवाद प्रकार का प्रतिनिधित्व करता है"
type: docs
weight: 2530
url: /hi/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

मानक आंतरिक अपवाद प्रकार का प्रतिनिधित्व करता है।

```csharp
public class TasksLoggedException : ApplicationException
```

## गुण

| नाम | विवरण |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | अपवाद लॉगिंग जानकारी प्राप्त करता है। |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | अपवाद ऑपरेशन जानकारी प्राप्त करता है। |

## उदाहरण

दिखाता है कि MPP निर्यात के साथ समस्याओं की जाँच के लिए लॉग टेक्स्ट और अपवाद प्रकार को कैसे पढ़ें।

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // परियोजना को MPP फ़ाइल के रूप में निर्यात करें
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


