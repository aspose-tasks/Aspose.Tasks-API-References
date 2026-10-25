---
title: "TaskUtils.TaskChildrenCount"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskUtils मेथड। सभी स्तरों पर टास्क के चाइल्ड टास्क की संख्या को पुनरावर्ती रूप से गणना करता है।"
type: docs
weight: 40
url: /hi/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

सभी स्तरों पर पुनरावर्ती रूप से टास्क के चाइल्ड टास्क की संख्या की गणना करता है।

```csharp
public static int TaskChildrenCount(Task task)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कार्य | कार्य | वह टास्क जिसे चाइल्ड्स गणना करते हैं। |

### रिटर्न वैल्यू

चाइल्ड्स की संख्या।

## उदाहरण

कैसे उपयोग करें &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt; मेथड दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// सभी स्तरों पर टास्क के चाइल्ड टास्क की संख्या को पुनरावर्ती रूप से गणना करता है
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### संबंधित देखें

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


