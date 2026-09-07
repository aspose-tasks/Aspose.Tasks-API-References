---
title: "क्लास CheckCircuit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.CheckCircuit क्लास। कार्यों के वृक्ष में सर्किट है या नहीं जांचता है।"
type: docs
weight: 2680
url: /hi/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

जाँचता है कि कार्यों के वृक्ष में कोई सर्किट है या नहीं।

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | `CheckCircuit` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | जाँचें कि निर्दिष्ट ऑब्जेक्ट पहले ही प्रोसेस किया गया है या नहीं। |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


