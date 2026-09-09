---
title: "Tsk.Contact"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevden sorumlu kişinin adı"
type: docs
weight: 220
url: /tr/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

Bir görevden sorumlu olan bireyin adı.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Örnekler

Tsk.Contact özelliğini nasıl okuyup/yazacağınızı gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


