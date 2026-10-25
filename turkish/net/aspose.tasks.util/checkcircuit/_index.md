---
title: "Sınıf CheckCircuit"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.CheckCircuit sınıfı. Görev ağacının bir devre içerip içermediğini kontrol eder"
type: docs
weight: 2680
url: /tr/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Görev ağacını (tree) bir devre içerip içermediğini kontrol eder.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | `CheckCircuit` sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Belirtilen nesnenin zaten işlenip işlenmediğini kontrol et. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


