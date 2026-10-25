---
title: "Tsk.PreleveledFinish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk field. Kaynak dengelemesi yapılmadan önce bir görevin bitiş tarihi"
type: docs
weight: 910
url: /tr/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

Kaynak dengelemesi yapılmadan önce bir görevin bitiş tarihi.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Örnekler

Tsk.PreleveledFinish özelliğini okuma/yazma nasıl gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


