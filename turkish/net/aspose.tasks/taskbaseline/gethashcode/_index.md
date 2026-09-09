---
title: "TaskBaseline.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskBaseline yöntemi. TaskBaseline sınıfının örneği için bir karma kod değeri döndürür"
type: docs
weight: 110
url: /tr/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

[`TaskBaseline`](../) sınıfının örneği için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir görev baseline'ının karma kodunu nasıl alacağınızı gösterir.

```csharp
var project = new Project();

// TaskBaseline oluşturma
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// görev baseline süresini görüntüle
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// Bir takvimin karma kodu baseline numarasına eşittir.
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### Ayrıca Bakınız

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


