---
title: "Project.Recalculate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, il lavoro e i campi di costo."
type: docs
weight: 1150
url: /it/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, i campi di lavoro e di costo.

```csharp
public void Recalculate()
```

## Esempi

Mostra come riprogrammare il progetto dalla data di inizio invece che da quella di fine.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// Ora tutte le date delle attività (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) sono calcolate. Per ottenere il percorso critico è necessario calcolare i margini (può essere invocato in un thread separato, ma solo dopo il calcolo di tutte le date anticipate/posticipate).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, i campi di lavoro e di costo con convalida opzionale.

```csharp
public void Recalculate(bool validate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| validate | Boolean | Se true la convalida della ricalcolazione verrà eseguita. Quali dati sono convalidati: al momento è implementata solo la convalida di base degli intervalli di date delle attività e dei collegamenti tra attività. Gli intervalli di date delle attività (ad es. ActualStart - ActualFinish, EarlyStart - EarlyFinish, ecc.) così come le date dei collegamenti tra attività saranno verificati rispetto al criterio che la data di inizio sia minore o uguale alla data di fine. Se una delle condizioni descritte sopra non è soddisfatta, verrà sollevata l'eccezione [`RecalculationValidationException`](../../recalculationvalidationexception/). |

## Esempi

Mostra come ricalcolare il progetto con convalida posteriore.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // ricalcolare il progetto con convalida posteriore
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


