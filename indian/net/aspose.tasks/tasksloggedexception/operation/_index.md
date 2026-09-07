---
title: "TasksLoggedException.Operation"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TasksLoggedException प्रॉपर्टी। अपवाद संचालन जानकारी प्राप्त करती है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

अपवाद ऑपरेशन जानकारी प्राप्त करता है।

```csharp
public string Operation { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


