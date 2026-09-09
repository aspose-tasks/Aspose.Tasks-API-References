---
title: "Tsk.PhysicalPercentComplete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Gerçekleşen işin bütçelenmiş maliyetini (BCWP) hesaplamak için alternatif olarak kullanılabilecek yüzde tamamlama değeri"
type: docs
weight: 900
url: /tr/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Gerçekleştirilen işin bütçelenen maliyetini (BCWP) hesaplamak için alternatif olarak kullanılabilecek yüzde tamamlama değeri.

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Örnekler

Tsk.PhysicalPercentComplete özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


