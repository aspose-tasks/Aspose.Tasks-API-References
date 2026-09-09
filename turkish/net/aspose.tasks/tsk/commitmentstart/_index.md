---
title: "Tsk.CommitmentStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir teslimatın başlangıç tarihi. Okuma yalnızca XML formatı için desteklenir."
type: docs
weight: 180
url: /tr/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

Teslimatın başlangıç tarihi. Okuma yalnızca XML formatı için desteklenir.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Örnekler

Tsk.CommitmentStart özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


