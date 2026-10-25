---
title: "Tsk.IsResumeValid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Tsk campo. Determina se un'attività può essere ripresa"
type: docs
weight: 680
url: /it/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Determina se un'attività può essere ripresa.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsResumeValid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


