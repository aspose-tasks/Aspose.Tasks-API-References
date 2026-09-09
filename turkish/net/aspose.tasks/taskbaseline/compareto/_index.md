---
title: "TaskBaseline.CompareTo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskBaseline yöntemi. IComparable arayüzü uygulaması. Bu örneği belirtilen Baseline nesnesiyle karşılaştırır"
type: docs
weight: 90
url: /tr/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

IComparable arabirimi uygulaması. Bu örneği belirtilen Baseline nesnesiyle karşılaştırır.

```csharp
public int CompareTo(TaskBaseline other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| diğer | TaskBaseline | bu örneğin karşılaştırılacağı belirtilen Baseline nesnesi. |

### Dönüş Değeri

belirtilen nesneden daha küçükse -1, daha büyükse 1 döndürür; aksi takdirde 0 döndürür

## Örnekler

Baseline'ların eşitliğini nasıl kontrol edeceğinizi gösterir.

```csharp
var project = new Project();

// TaskBaseline oluşturma
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// görev baseline süresini görüntüle
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// Baseline'ların eşitliği, baseline sayılarına karşı kontrol edilir.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Ayrıca Bakınız

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


