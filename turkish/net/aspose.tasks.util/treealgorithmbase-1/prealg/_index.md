---
title: "TreeAlgorithmBase1.PreAlg"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TreeAlgorithmBase yöntemi. Bir ağacın düğümünün işlenmesinden önce çağrılır."
type: docs
weight: 30
url: /tr/net/aspose.tasks.util/treealgorithmbase-1/prealg/
---
## TreeAlgorithmBase&lt;T&gt;.PreAlg method

Bir ağacın düğümünün işlenmesinden önce çağrılır.

```csharp
public virtual void PreAlg(T el, int level)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | İşlenecek düğüm. |
| seviye | Int32 | Ağaç düğüm seviyesi. |

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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


