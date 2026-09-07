---
title: "Tsk.StatusManager"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il nome della risorsa aziendale che deve ricevere gli aggiornamenti di stato per l'attività corrente dalle risorse"
type: docs
weight: 1050
url: /it/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

Il nome della risorsa aziendale che deve ricevere gli aggiornamenti di stato per l'attività corrente dalle risorse.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.StatusManager.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


