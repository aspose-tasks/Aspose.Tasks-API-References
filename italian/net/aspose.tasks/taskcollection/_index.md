---
title: Class TaskCollection
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.TaskCollection classe. Rappresenta una raccolta diTask oggetti.
type: docs
weight: 2100
url: /it/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Rappresenta una raccolta di[`Task`](../task/) oggetti.

```csharp
public class TaskCollection : IList<Task>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Ottiene il numero di oggetti contenuti nella TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Ottiene un valore che indica se questa raccolta è di sola lettura. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Ottiene il progetto principale dell'oggetto TaskCollection. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Aggiunge una nuova attività alla raccolta di attività del progetto sullo stesso livello di struttura dell'ultima attività. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Inserisce una nuova attività prima di un'attività con l'id specificato e sullo stesso livello di struttura. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Aggiunge una nuova attività alla raccolta di attività figlio. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Aggiunge l'attività specificata all'istanza di`TaskCollection`class. Se ParentProject.CalculationMode è None, l'utente deve richiamare Project.Recalculate() dopo aver utilizzato questo metodo (ripianificherà tutte le attività del progetto (date di inizio/fine, imposta date anticipate/ritardate) e calcolerà i campi dipendenti come tempi di attesa, lavoro e campi di costo, ID e livelli di struttura). Se ParentProject.CalculationMode è Manuale, il metodo calcolerà automaticamente solo l'ID attività, il livello di struttura e i numeri di struttura. Se ParentProject.CalculationMode è Automatico, il metodo ripianifica automaticamente tutte le attività del progetto (inizio/fine date, imposta le date anticipate/posteriori, calcola gli spazi vuoti, i campi di lavoro e di costo, ricalcola gli ID e i livelli di struttura). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Aggiunge una nuova attività ricorrente alla raccolta di attività per bambini. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Verifica se la raccolta contiene l'elemento specificato. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Restituisce un'attività con l'ID specificato il cui predecessore è l'attività principale di questa raccolta . |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Restituisce un'attività con l'Uid specificato il cui predecessore è l'attività padre di questa raccolta . |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Restituisce un enumeratore per questa raccolta. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Questa è l'implementazione stub del metodo Insert di IList, che genera solo NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Questa è l'implementazione stub del metodo Remove di ICollection, che genera solo NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Converte l'oggetto TaskCollection in un elenco di[`Task`](../task/) oggetti. |

### Guarda anche

* class [Task](../task/)
* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


