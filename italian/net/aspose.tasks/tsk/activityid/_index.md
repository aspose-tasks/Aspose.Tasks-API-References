---
title: "Tsk.ActivityId"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Rappresenta il campo ID attività, un identificatore unico dell'attività utilizzato da Primavera. Applicabile solo ai progetti Primavera"
type: docs
weight: 10
url: /it/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Rappresenta il campo ID attività - l'identificatore univoco di un'attività usato da Primavera. (applicabile solo ai progetti Primavera).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Esempi

Mostra come lavorare con il campo ActivityId specifico per i progetti Primavera

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// crea le opzioni di salvataggio Primavera e specifica che gli ActivityId non devono essere sovrascritti durante il salvataggio.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


