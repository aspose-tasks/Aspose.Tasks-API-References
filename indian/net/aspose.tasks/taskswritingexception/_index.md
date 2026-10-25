---
title: "क्लास TasksWritingException"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TasksWritingException क्लास। मानक आंतरिक लेखन अपवाद प्रकार का प्रतिनिधित्व करता है।"
type: docs
weight: 2560
url: /hi/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

मानक आंतरिक लिखने के अपवाद प्रकार का प्रतिनिधित्व करता है।

```csharp
public class TasksWritingException : TasksLoggedException
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

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


