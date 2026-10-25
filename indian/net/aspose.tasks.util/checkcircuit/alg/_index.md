---
title: "CheckCircuit.Alg"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CheckCircuit method. निर्दिष्ट वस्तु पहले ही प्रक्रिया की गई है या नहीं जाँचें।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

जाँचें कि निर्दिष्ट ऑब्जेक्ट पहले ही प्रोसेस किया गया है या नहीं।

```csharp
public override void Alg(Task el, int level)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | कार्य | प्रक्रिया करने के लिए वस्तु। |
| स्तर | Int32 | पेड़ नोड का स्तर। |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


