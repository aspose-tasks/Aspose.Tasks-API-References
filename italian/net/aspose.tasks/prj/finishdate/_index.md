---
title: "Prj.FinishDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La data di fine di un progetto"
type: docs
weight: 330
url: /it/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

La data di fine di un progetto.

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
```

## Esempi

Mostra come riprogrammare il progetto dalla data di fine invece che da quella di inizio.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// Ora tutte le date delle attività (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) sono calcolate. Per ottenere il percorso critico è necessario calcolare i margini (può essere invocato in un thread separato, ma solo dopo il calcolo di tutte le date anticipate/posticipate).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


