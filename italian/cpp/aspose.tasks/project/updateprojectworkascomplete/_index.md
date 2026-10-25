---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete metodo"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks per C++"
description: "Aggiorna tutto il lavoro come completato fino a una data specificata per l'intero progetto."
type: docs
weight: 2080
url: /it/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Aggiorna tutto il lavoro come completato fino a una data specificata per l'intero progetto.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Parametro | Descrizione |
| --- | --- |
| completeThrough | La data fino a cui aggiornare il lavoro come completato. |
| setZeroOrHundredPercentCompleteOnly | Se impostato su true aggiorna solo le attività al 100% completate la cui data di fine è precedente alla data di completamento specificata. Altrimenti, calcola un valore percentuale di completamento basato sulle date di inizio programmate e di completamento. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Aggiorna tutto il lavoro come completato fino a una data specificata per l'elenco specificato di attività.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Parametro | Descrizione |
| --- | --- |
| completeThrough | La data fino a cui aggiornare il lavoro come completato. |
| setZeroOrHundredPercentCompleteOnly | Se impostato su true aggiorna solo le attività al 100% completate la cui data di fine è precedente alla data di completamento specificata. Altrimenti, calcola un valore percentuale di completamento basato sulle date di inizio programmate e di completamento. |
| taskCollection | Elenco< Task > delle attività per le quali aggiornare il lavoro. |

