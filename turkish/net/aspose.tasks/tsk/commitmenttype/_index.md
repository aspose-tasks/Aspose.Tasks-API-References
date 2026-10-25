---
title: "Tsk.CommitmentType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin ilişkili bir teslimatı olup olmadığını veya ilişkili bir teslimata bağımlılığı olup olmadığını belirler. Okuma yalnızca XML formatı için desteklenir."
type: docs
weight: 190
url: /tr/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Bir görevin ilişkili bir teslimatı olup olmadığını veya ilişkili bir teslimata bağımlılığı olup olmadığını belirler. Okuma yalnızca XML formatı için desteklenir.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Örnekler

Tsk.CommitmentType özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


