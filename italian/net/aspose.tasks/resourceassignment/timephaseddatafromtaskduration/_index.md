---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceAssignment. Genera un elenco di dati a intervalli temporali basato sulla durata dell'attività e sulla data di inizio pianificata"
type: docs
weight: 780
url: /it/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

Genera un elenco di dati a intervalli temporali basato sulla durata dell'attività e sulla data di inizio programmata.

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calendario | Calendar | Il calendario da cui generare i dati a intervalli temporali. |

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


