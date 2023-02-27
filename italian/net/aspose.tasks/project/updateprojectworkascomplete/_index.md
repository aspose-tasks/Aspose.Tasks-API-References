---
title: Project.UpdateProjectWorkAsComplete
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Project metodo. Aggiorna tutto il lavoro come completato fino a una data specificata per lintero progetto.
type: docs
weight: 1250
url: /it/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

Aggiorna tutto il lavoro come completato fino a una data specificata per l'intero progetto.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| completeThrough | DateTime | La data per aggiornare il lavoro come completato. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Se impostato su true, aggiorna solo le attività completate al 100% la cui data di fine è precedente alla data di completamento specificata. In caso contrario, calcola un valore percentuale di completamento basato sulle date di inizio e di completamento pianificate. |

### Guarda anche

* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

Aggiorna tutto il lavoro come completato fino a una data specificata per l'elenco di attività specificato.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| completeThrough | DateTime | La data per aggiornare il lavoro come completato. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Se impostato su true, aggiorna solo le attività completate al 100% la cui data di fine è precedente alla data di completamento specificata. In caso contrario, calcola un valore percentuale di completamento basato sulle date di inizio e di completamento pianificate. |
| taskCollection | List`1 | Elenco&lt;attività&gt; di attività per cui aggiornare il lavoro. |

### Guarda anche

* class [Task](../../task/)
* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)


