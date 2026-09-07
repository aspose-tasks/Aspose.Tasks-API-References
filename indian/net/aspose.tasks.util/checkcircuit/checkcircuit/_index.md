---
title: "CheckCircuit.CheckCircuit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CheckCircuit constructor. CheckCircuit वर्ग का नया उदाहरण आरंभ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

[`CheckCircuit`](../) वर्ग का नया उदाहरण आरंभ करता है।

```csharp
public CheckCircuit()
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

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


