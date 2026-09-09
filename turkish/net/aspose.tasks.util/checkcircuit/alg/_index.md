---
title: "CheckCircuit.Alg"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CheckCircuit yöntemi. Belirtilen nesnenin zaten işlenip işlenmediğini kontrol eder"
type: docs
weight: 20
url: /tr/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Belirtilen nesnenin zaten işlenip işlenmediğini kontrol et.

```csharp
public override void Alg(Task el, int level)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | Görev | İşlenecek nesne. |
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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


