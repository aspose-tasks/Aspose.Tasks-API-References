---
title: "Tsk.Contact"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il nome di una persona responsabile di un'attività"
type: docs
weight: 220
url: /it/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

Il nome di un individuo responsabile di un'attività.

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.Contact.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


