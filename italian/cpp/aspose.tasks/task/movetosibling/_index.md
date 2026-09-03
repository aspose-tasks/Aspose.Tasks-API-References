---
title: "Aspose::Tasks::Task::MoveToSibling metodo"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks per C++"
description: "Sposta l'attività corrente allo stesso livello di struttura prima dell'attività specificata."
type: docs
weight: 1370
url: /it/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Sposta l'attività corrente allo stesso livello di outline prima dell'attività specificata. Se ParentProject.CalculationMode è None, l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate) e calcolerà i campi dipendenti come slacks, lavoro e costi, i livelli di outline). Se ParentProject.CalculationMode è Manual, il metodo calcolerà automaticamente solo l'ID dell'attività, il livello di outline e i numeri di outline. Se ParentProject.CalculationMode è Automatic, il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate, calcola slacks, lavoro e costi, ricalcola gli ID e i livelli di outline).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Parametro | Descrizione |
| --- | --- |
| beforeTask | Attività prima della quale verrà inserita l'attività corrente. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Sposta l'attività corrente allo stesso livello di struttura prima di un'attività con l'Id specificato. Se ParentProject.CalculationMode è None, l'utente dovrebbe invocare Project.Recalculate() dopo aver usato questo metodo (Riprogrammerà tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate) e calcolerà i campi dipendenti come i margini, i campi di lavoro e di costo, i livelli di struttura). Se ParentProject.CalculationMode è Manual, il metodo calcolerà solo l'Id dell'attività, il livello di struttura e i numeri di struttura automaticamente. Se ParentProject.CalculationMode è Automatic, il metodo riprogramma automaticamente tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, i campi di lavoro e di costo, ricalcola gli Id e i livelli di struttura).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Parametro | Descrizione |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) di un'attività prima della quale verrà inserita l'attività corrente. |

