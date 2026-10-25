---
title: "TaskCollection"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 1140
url: /it/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Rappresenta una raccolta di [Task](/tasks/python-net/aspose.tasks/task/) oggetti.

Il tipo TaskCollection espone i seguenti membri:
## Proprietà
| Nome | Descrizione |
| :- | :- |
| parent_project | Ottiene il progetto padre dell'oggetto TaskCollection. |
## Methods
| Nome | Descrizione |
| :- | :- |
| add() | Aggiunge il task specificato all'istanza della classe [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/).<br/>            Se ParentProject.CalculationMode è None, l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutti i task del progetto (date di inizio/fine, imposta le date anticipate/posticipate) e calcolerà i campi dipendenti come slacks, lavoro e costi, ID e livelli di outline).<br/>            Se ParentProject.CalculationMode è Manual, il metodo calcolerà solo l'ID del task, il livello di outline e i numeri di outline automaticamente.<br/>            Se ParentProject.CalculationMode è Automatic, il metodo riprogramma automaticamente tutti i task del progetto<br/>            (date di inizio/fine, imposta le date anticipate/posticipate, calcola slacks, lavoro e costi, ricalcola gli ID e i livelli di outline). |
| add(task_name) | Aggiunge un nuovo task alla collezione dei task figli. |
| add(task_name, before_task_id) |  |
| add(parameters) | Inserisce un nuovo task prima di un task con l'ID specificato e allo stesso livello di outline. |
| to_list() | Converte l'oggetto TaskCollection in un elenco di oggetti [Task](/tasks/python-net/aspose.tasks/task/). |
| get_by_uid(uid) | Restituisce un task con l'Uid specificato il cui antenato è il task padre di questa collezione . |
| get_by_id(id) | Restituisce un task con l'Id specificato il cui antenato è il task padre di questa collezione . |

### Vedi anche

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

