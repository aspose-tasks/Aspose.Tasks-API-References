---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di GraphicalIndicatorCriteria. Inizializza una nuova istanza del tipo GraphicalIndicatorCriteria"
type: docs
weight: 10
url: /it/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Inizializza una nuova istanza del tipo [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | valore dell'enumerazione [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) che indica per quali righe viene applicato l'indicatore |
| test | FilterComparisonType | valore di [`FilterComparisonType`](../../filtercomparisontype/) che denota il tipo di confronto eseguito dal criterio. |
| imageIndex | Int32 | l'indice dell'immagine da visualizzare quando il campo soddisfa i criteri |
| value1 | GraphicalIndicatorCriteriaValue | valori usati nel controllo della condizione. |
| value2 | GraphicalIndicatorCriteriaValue | secondo valore (fine dell'intervallo) usato nel controllo della condizione nei casi di condizioni 'IsWithin' e 'IsNotWithing'. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Generato quando viene passata una combinazione errata di argomenti al costruttore. |

### Vedi anche

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Inizializza una nuova istanza del tipo [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | valore dell'enumerazione [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) che indica per quali righe viene applicato l'indicatore |
| test | FilterComparisonType | valore di [`FilterComparisonType`](../../filtercomparisontype/) che denota il tipo di confronto eseguito dal criterio. |
| imageIndex | Int32 | l'indice dell'immagine da visualizzare quando il campo soddisfa i criteri |
| valore | GraphicalIndicatorCriteriaValue | valore usato nel controllo della condizione. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Generato quando viene passata una combinazione errata di argomenti al costruttore. |
| ArgumentException | Quando il valore di IsWithin o IsNotWithing viene passato all'argomento di test. |

### Vedi anche

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


