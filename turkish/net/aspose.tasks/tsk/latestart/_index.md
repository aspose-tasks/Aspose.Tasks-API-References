---
title: "Tsk.LateStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin projenin bitişini geciktirmeden başlayabileceği en son tarih"
type: docs
weight: 740
url: /tr/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

Bir görevin projenin bitişini geciktirmeden başlayabileceği en son tarih.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Örnekler

Tsk.LateStart özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


