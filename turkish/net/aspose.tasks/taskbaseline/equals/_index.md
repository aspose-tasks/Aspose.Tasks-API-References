---
title: "TaskBaseline.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskBaseline yöntemi. Bu örneğin belirtilen TaskBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür"
type: docs
weight: 100
url: /tr/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Bu örneğin belirtilen TaskBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(TaskBaseline other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| diğer | TaskBaseline | bu örnekle karşılaştırmak için belirtilen AssignmentBaseline nesnesi. |

### Dönüş Değeri

Bu örnek belirtilen TaskBaseline nesnesine eşitse true, aksi takdirde false döndürür.

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

---

## Equals(object) {#equals_2}

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnekle karşılaştırılacak nesne. |

### Dönüş Değeri

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

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


