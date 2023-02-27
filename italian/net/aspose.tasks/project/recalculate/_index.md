---
title: Project.Recalculate
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Project metodo. Riprogramma tutti gli ID delle attività del progetto i livelli di struttura le date di inizio/fine imposta le date di inizio/fine calcola i campi di lavoro e di costo.
type: docs
weight: 1120
url: /it/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date di inizio/fine, calcola i campi di lavoro e di costo.

```csharp
public void Recalculate()
```

### Guarda anche

* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Riprogramma tutti gli ID delle attività del progetto, i livelli di struttura, le date di inizio/fine, imposta le date di inizio/fine, calcola i campi di lavoro e di costo con convalida facoltativa.

```csharp
public void Recalculate(bool validate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| validate | Boolean | Se true, verrà eseguita la convalida del ricalcolo. Quali dati vengono convalidati: Al momento è implementata solo la convalida di base degli intervalli di date delle attività e dei collegamenti alle attività. Gli intervalli di date delle attività (ad es. ActualStart - ActualFinish, EarlyStart - EarlyFinish, ecc. ) così come le date dei collegamenti attività verranno verificate in base ai criteri di data secondo cui la data di inizio è inferiore o uguale alla data di fine. Se una delle condizioni sopra descritte non è riuscita, allora[`RecalculationValidationException`](../../recalculationvalidationexception/)verrà lanciato. |

### Guarda anche

* class [Project](../)
* spazio dei nomi [Aspose.Tasks](../../project/)
* assemblea [Aspose.Tasks](../../../)


