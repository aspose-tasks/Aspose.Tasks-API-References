---
title: "ResourceAssignment.SplitTask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceAssignment. Divide l'attività in due parti"
type: docs
weight: 770
url: /it/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Dividi l'attività in due parti.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | L'inizio dell'interruzione del lavoro su cui basare la divisione. |
| fine | DateTime | La fine dell'interruzione del lavoro su cui basare la divisione. |
| calendario | Calendar | Il calendario su cui basare la divisione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | Genera un'eccezione quando la data di inizio è inferiore alla data di inizio dell'assegnazione. |
| ArgumentOutOfRangeException | Genera un'eccezione quando la data di fine è superiore alla data di fine dell'assegnazione. |

## Esempi

Mostra come aggiungere una divisione a un'attività.

```csharp
var project = new Project();

// Ottieni un calendario standard
var calendar = project.Get(Prj.Calendar);

// Imposta le impostazioni del calendario del progetto
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Aggiungi una nuova attività all'attività radice
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Crea una nuova assegnazione di risorsa e genera dati a intervalli temporali
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Dividi l'attività in 3 parti.
// Fornisci gli argomenti data di inizio e data di fine al metodo SplitTask che verranno usati per la divisione
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


