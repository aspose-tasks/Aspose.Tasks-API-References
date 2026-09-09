---
title: "Tsk.EarlyStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Önceki ve sonraki görevlerin erken başlangıç tarihleri ve diğer kısıtlamalar temelinde bir görevin başlayabileceği en erken tarih."
type: docs
weight: 340
url: /tr/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

Önceki ve sonraki görevlerin erken başlangıç tarihleri ve diğer kısıtlamalar temel alınarak bir görevin mümkün olan en erken başlangıç tarihi.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Örnekler

Tsk.EarlyStart özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


