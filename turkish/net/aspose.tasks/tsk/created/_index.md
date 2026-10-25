---
title: "Tsk.Created"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin oluşturulduğu tarih."
type: docs
weight: 250
url: /tr/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

Bir görevin oluşturulduğu tarih.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Örnekler

Tsk.Created özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


