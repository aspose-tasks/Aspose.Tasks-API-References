---
title: "Tsk.Contact"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Имя лица, ответственного за задачу"
type: docs
weight: 220
url: /ru/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

Имя лица, ответственного за задачу.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.Contact.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


