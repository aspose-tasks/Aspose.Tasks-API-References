---
title: "CheckCircuit.CheckCircuit"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CheckCircuit yapıcı. CheckCircuit sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

[`CheckCircuit`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public CheckCircuit()
```

## Örnekler

Bozuk bir projenin yapısını nasıl tespit edeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// projenin yapısını kontrol et.
// Proje yapısı hatalıysa <see cref=\"TasksException\"> fırlatılacaktır.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Ayrıca Bakınız

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


