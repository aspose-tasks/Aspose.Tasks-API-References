---
title: "Tsk.EarlyFinish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin, önceki ve sonraki görevlerin erken bitiş tarihleri, diğer kısıtlamalar ve herhangi bir dengeleme gecikmesi temelinde mümkün olan en erken bitiş tarihi"
type: docs
weight: 330
url: /tr/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

Önceki ve sonraki görevlerin erken bitiş tarihleri, diğer kısıtlamalar ve olası dengeleme gecikmesi temel alınarak bir görevin mümkün olan en erken bitiş tarihi.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Örnekler

Tsk.EarlyFinish özelliğini nasıl okuyup/yazacağınızı gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


