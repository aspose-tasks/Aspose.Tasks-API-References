---
title: "Tsk.Deadline"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk field. Bir görevin ne zaman tamamlanacağını gösteren hedef tarih"
type: docs
weight: 270
url: /tr/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

Bir görevin tamamlanması gereken tarihi gösteren hedef tarih.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Örnekler

Tsk.Deadline özelliğini okuma/yazma gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


