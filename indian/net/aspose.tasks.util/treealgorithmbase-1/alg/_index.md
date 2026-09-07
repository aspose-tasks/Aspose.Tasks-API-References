---
title: "TreeAlgorithmBase1.Alg"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TreeAlgorithmBase मेथड। पेड़ के एक नोड को प्रोसेस करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/treealgorithmbase-1/alg/
---
## TreeAlgorithmBase&lt;T&gt;.Alg method

ट्री के एक नोड को प्रोसेस करता है।

```csharp
public abstract void Alg(T el, int level)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रोसेस करने के लिए नोड। |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


