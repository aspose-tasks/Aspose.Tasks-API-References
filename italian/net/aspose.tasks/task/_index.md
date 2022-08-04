---
title: Task
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Rappresenta unattività in un progetto.
type: docs
weight: 2060
url: /it/net/aspose.tasks/task/
---
## Task class

Rappresenta un'attività in un progetto.

```csharp
public class Task : IEquatable<Task>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | Ottiene una raccolta di assegnazioni di risorse per questo oggetto. |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | Ottiene o imposta la raccolta dei valori di base dell'attività. |
| [Children](../../aspose.tasks/task/children) { get; } | Ottiene una raccolta di attività figlio di questo oggetto. Oggetto TaskCollection che rappresenta le attività figlio. |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | Ottiene l'oggetto ExtendedAttributeCollection contenente i valori di un attributo esteso. |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | Ottiene o imposta[`OutlineCodeCollection`](../outlinecodecollection) oggetto. |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | Ottiene il progetto padre di un'attività. |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | Ottiene l'attività padre di un'attività. |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | Ottiene a[`TaskCollection`](../taskcollection) oggetto che contiene tutti i predecessori di questo oggetto Task. |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | Ottiene l'istanza di[`RecurringTaskInfo`](../recurringtaskinfo) classe per l'attività che è un'attività ricorrente; se l'attività non è ricorrente, restituisce null;  Le informazioni per l'istanza di[`RecurringTaskInfo`](../recurringtaskinfo) è presente solo in formato file mpp. |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | Ottiene una raccolta SplitPart che rappresenta le parti di un'attività. |
| [Successors](../../aspose.tasks/task/successors) { get; } | Ottiene a[`TaskCollection`](../taskcollection) oggetto che contiene tutti i successori di questo oggetto Task. |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | Ottiene o imposta un oggetto TimephasedDataCollection di questa attività. Il blocco di dati in fasi temporali associato a un'attività. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | Crea la copia completa di un'attività senza attività secondarie. |
| [Delete](../../aspose.tasks/task/delete)() | Elimina un'attività dalla raccolta di attività del progetto padre e tutte le relative assegnazioni. |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | Restituisce un valore che indica se questa istanza è uguale a un'attività specificata. |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | Restituisce il valore a cui è mappata la proprietà in questo contenitore. |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | Restituisce un valore di codice hash per questa attività. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | Restituisce[`TimephasedDataCollection`](../timephaseddatacollection) oggetto con[`TimephasedData`](./timephaseddata) valori entro date di inizio e fine date. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | Restituisce[`TimephasedDataCollection`](../timephaseddatacollection) oggetto con[`TimephasedData`](./timephaseddata) valori entro date di inizio e fine specificate del tipo di dati in fasi temporali specificato. |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | Sposta l'attività corrente allo stesso livello struttura prima di un'attività con l'ID specificato. Se ParentProject.CalculationMode è None l'utente deve richiamare Project.Recalculate() dopo aver utilizzato questo metodo (ripianificherà tutte le attività del progetto (date di inizio/fine, imposta le date di inizio/fine) e calcola i campi dipendenti come spazi liberi, campi di lavoro e costi, livelli struttura). Se ParentProject.CalculationMode è Manuale, il metodo calcolerà automaticamente solo l'ID attività, il livello struttura e i numeri struttura. Se ParentProject. CalculationMode è Automatico, il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta le date di inizio/fine, calcola i campi di lavoro e di costo, ricalcola gli ID e i livelli di struttura). |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | Sposta l'attività corrente allo stesso livello struttura prima dell'attività specificata. Se ParentProject.CalculationMode è None l'utente deve richiamare Project.Recalculate() dopo aver utilizzato questo metodo (ripiancherà tutte le attività del progetto (date di inizio/fine, imposta in anticipo/ date di ritardo) e calcolerà i campi dipendenti come slack, campi di lavoro e costi, livelli struttura). Se ParentProject.CalculationMode è Manuale, il metodo calcolerà automaticamente solo l'ID attività, il livello struttura e i numeri struttura. Se ParentProject.CalculationMode è Automatico il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta le date di inizio/fine, calcola gli slack, i campi di lavoro e di costo, ricalcola gli ID e i livelli di struttura). |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | Rientra un'attività nella struttura. |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | Promuove un'attività nella struttura. |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | Raccoglie ricorsivamente tutte le attività figlio di questa attività. |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | Mappa la proprietà specificata sul valore specificato in questo contenitore. |
| override [ToString](../../aspose.tasks/task/tostring)() | Restituisce la rappresentazione di una stringa breve di un'attività. I dettagli esatti della rappresentazione non sono specificati e sono soggetti a modifiche. |

### Osservazioni

Il **Compito** rappresenta un mandrino di lavoro atomico.

Si può usare **Compito**per pianificare un progetto creando attività e assegnando loro risorse appropriate. Le attività in un progetto sono organizzate come una struttura ad albero gerarchico radicata, con un'attività radice e sottostrutture di attività figlio.

Per costruire un albero di attività è possibile utilizzare una raccolta specializzata[`TaskCollection`](../taskcollection) accedendo[`RootTask`](../project/roottask) proprietà es:

```csharp
Project project = new Project();

// aggiungi nuove attività
Task task1 = project.RootTask.Children.Add(); // viene aggiunta un'attività padre con un nome vuoto
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // inserisce un'attività prima di childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// salva il progetto in uno dei formati disponibili
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks)
* assemblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
