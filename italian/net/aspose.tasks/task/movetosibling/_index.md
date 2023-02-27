---
title: Task.MoveToSibling
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Task metodo. Sposta lattività corrente allo stesso livello struttura prima dellattività specificata. Se ParentProject.CalculationMode è None lutente deve richiamare Project.Recalculate dopo aver utilizzato questo metodo ripianificherà tutte le attività del progetto date di inizio/fine imposta anticipatamente/ date in ritardo e calcolare i campi dipendenti come la flessibilità i campi di lavoro e di costo i livelli di struttura. Se ParentProject.CalculationMode è Manuale il metodo calcolerà automaticamente solo lID attività il livello di struttura e i numeri di struttura. Se ParentProject.CalculationMode è Automatico il metodo ripianifica automaticamente tutte le attività del progetto date di inizio/fine imposta date di inizio/fine calcola i campi di lavoro e di costo ricalcola gli ID e i livelli di struttura.
type: docs
weight: 1370
url: /it/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Sposta l'attività corrente allo stesso livello struttura prima dell'attività specificata. Se ParentProject.CalculationMode è None, l'utente deve richiamare Project.Recalculate() dopo aver utilizzato questo metodo (ripianificherà tutte le attività del progetto (date di inizio/fine, imposta anticipatamente/ date in ritardo) e calcolare i campi dipendenti come la flessibilità, i campi di lavoro e di costo, i livelli di struttura). Se ParentProject.CalculationMode è Manuale, il metodo calcolerà automaticamente solo l'ID attività, il livello di struttura e i numeri di struttura. Se ParentProject.CalculationMode è Automatico il metodo ripianifica automaticamente tutte le attività del progetto (date di inizio/fine, imposta date di inizio/fine, calcola i campi di lavoro e di costo, ricalcola gli ID e i livelli di struttura).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| beforeTask | Task | Attività prima della quale verrà inserita l'attività corrente. |

### Guarda anche

* class [Task](../)
* spazio dei nomi [Aspose.Tasks](../../task/)
* assemblea [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Sposta l'attività corrente allo stesso livello struttura prima di un'attività con l'ID specificato. Se ParentProject.CalculationMode è None, l'utente deve richiamare Project.Recalculate() dopo aver utilizzato questo metodo (ripianificherà tutte le attività del progetto (date di inizio/fine, imposta le date anticipate/tardive) e calcola i campi dipendenti come la flessibilità, i campi di lavoro e di costo, i livelli di struttura). Se ParentProject.CalculationMode è impostato su Manual, il metodo calcolerà automaticamente solo ID attività, livello di struttura e numeri di struttura. Se ParentProject. CalculationMode è Automatico il metodo ripianifica automaticamente tutte le attività del progetto (date di inizio/fine, imposta date di anticipo/ritardo, calcola i campi di lavoro e di costo, ricalcola gli ID e i livelli di struttura).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| beforeTaskId | Int32 | Id ([`Id`](../../tsk/id/)) di un'attività prima della quale verrà inserita l'attività corrente. |

### Guarda anche

* class [Task](../)
* spazio dei nomi [Aspose.Tasks](../../task/)
* assemblea [Aspose.Tasks](../../../)


