---
title: "Tsk.LateFinish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin projenin bitişini geciktirmeden tamamlayabileceği en son tarih"
type: docs
weight: 730
url: /tr/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

Bir görevin projenin bitişini geciktirmeden tamamlanabileceği en son tarih.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Örnekler

Tsk.LateFinish özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


