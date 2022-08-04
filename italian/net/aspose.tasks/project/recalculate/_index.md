---
title: Recalculate
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Riprogramma tutti gli ID delle attività del progetto i livelli di struttura le date di inizio/fine imposta le date di inizio/fine calcola i campi di lavoro di lavoro e di costo.
type: docs
weight: 340
url: /it/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date di inizio/fine, calcola i campi di lavoro, di lavoro e di costo.

```csharp
public void Recalculate()
```

### Guarda anche

* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date di inizio/fine, calcola i campi di lavoro e costi con la convalida opzionale.

```csharp
public void Recalculate(bool validate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| validate | Boolean | Se true verrà eseguita la convalida del ricalcolo. Quali dati vengono convalidati: Al momento è implementata solo la convalida di base degli intervalli di date di collegamento attività e attività. Intervalli di date dell'attività (ad es. ActualStart - ActualFinish, EarlyStart - EarlyFinish, ecc. ) così come le date dei collegamenti alle attività verranno verificate rispetto ai criteri di data in cui la data di inizio è inferiore o uguale alla data di fine. Se una qualsiasi delle condizioni sopra descritte non è soddisfatta,[`RecalculationValidationException`](../../recalculationvalidationexception) verrà lanciato. |

### Guarda anche

* class [Project](../../project)
* spazio dei nomi [Aspose.Tasks](../../project)
* assemblea [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->