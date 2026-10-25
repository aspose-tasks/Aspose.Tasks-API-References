---
title: "Task.MoveToSibling"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Sposta l'attività corrente allo stesso Outline Level prima dell'attività specificata. Se ParentProject.CalculationMode è None l'utente dovrebbe invocare Project.Recalculate dopo aver usato questo metodo. Riprogrammerà le date di inizio/fine di tutte le attività del progetto, imposterà le date early/late e calcolerà i campi dipendenti come slacks, work e cost nei livelli di Outline. Se ParentProject.CalculationMode è Manual il metodo calcolerà solo l'ID dell'attività, il livello di Outline e i numeri di Outline automaticamente. Se ParentProject.CalculationMode è Automatic il metodo riprogrammerà automaticamente le date di inizio/fine di tutte le attività del progetto, imposterà le date early/late, calcolerà slacks, work e cost, ricalcolerà gli ID e i livelli di Outline"
type: docs
weight: 1370
url: /it/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Sposta l'attività corrente allo stesso Livello di Contorno prima dell'attività specificata. Se ParentProject.CalculationMode è None l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutte le attività del progetto (date di inizio/fine, imposta date anticipate/posticipate) e calcolerà i campi dipendenti come scarti, lavoro e costi, livelli di contorno). Se ParentProject.CalculationMode è Manual il metodo calcolerà automaticamente solo l'id dell'attività, il livello di contorno e i numeri di contorno. Se ParentProject.CalculationMode è Automatic il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta date anticipate/posticipate, calcola scarti, lavoro e costi, ricalcola id e livelli di contorno).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| beforeTask | Attività | Task prima del quale verrà inserita l'attività corrente. |

## Esempi

Mostra come spostare l'attività sotto lo stesso genitore.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Sposta le attività con id 5 prima dell'attività con id 3
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// OPPURE
// Sposta l'attività alla fine della collezione
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Sposta l'attività corrente allo stesso Livello di Contorno prima di un'attività con l'Id specificato. Se ParentProject.CalculationMode è None l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutte le attività del progetto (date di inizio/fine, imposta date anticipate/posticipate) e calcolerà i campi dipendenti come scarti, lavoro e costi, livelli di contorno). Se ParentProject.CalculationMode è Manual il metodo calcolerà automaticamente solo l'id dell'attività, il livello di contorno e i numeri di contorno. Se ParentProject.CalculationMode è Automatic il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta date anticipate/posticipate, calcola scarti, lavoro e costi, ricalcola id e livelli di contorno).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| beforeTaskId | Int32 | Id ([`Id`](../../tsk/id/)) di un'attività prima della quale verrà inserita l'attività corrente. |

## Esempi

Mostra come spostare l'attività sotto lo stesso genitore usando l'Id dell'attività.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Sposta le attività con id 5 prima dell'attività con id 3
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// OPPURE
// Sposta l'attività alla fine della collezione
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


