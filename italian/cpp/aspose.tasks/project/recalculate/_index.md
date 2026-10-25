---
title: "Aspose::Tasks::Project::Recalculate metodo"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "Aspose.Tasks per C++"
description: "Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, i campi di lavoro e di costo."
type: docs
weight: 1130
url: /it/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini, i campi di lavoro e di costo.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date anticipate/posticipate, calcola i margini di tempo, i campi di lavoro e di costo con convalida opzionale.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| Parametro | Descrizione |
| --- | --- |
| valida | Se vero, verrà eseguita la convalida del ricalcolo. Quali dati vengono convalidati: al momento è implementata solo la convalida di base degli intervalli di date delle attività e dei collegamenti tra attività. Gli intervalli di date delle attività (ad es. ActualStart - ActualFinish, EarlyStart - EarlyFinish, ecc.) così come le date dei collegamenti tra attività saranno verificati rispetto al criterio che la data di inizio sia minore o uguale alla data di fine. Se una delle condizioni descritte sopra non è soddisfatta, verrà sollevata l'eccezione RecalculationValidationException. |

