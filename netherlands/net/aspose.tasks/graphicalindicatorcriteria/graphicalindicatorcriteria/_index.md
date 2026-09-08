---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GraphicalIndicatorCriteria constructor. Initialiseert een nieuw exemplaar van het GraphicalIndicatorCriteria-type."
type: docs
weight: 10
url: /nl/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Initialiseert een nieuw exemplaar van het [`GraphicalIndicatorCriteria`](../) type.

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | waarde van de [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) enum die aangeeft op welke rijen de indicator wordt toegepast. |
| test | FilterComparisonType | waarde van de [`FilterComparisonType`](../../filtercomparisontype/) die het type vergelijking aangeeft dat door de criteria wordt uitgevoerd. |
| imageIndex | Int32 | de index van de afbeelding die moet worden weergegeven wanneer het veld aan de criteria voldoet. |
| value1 | GraphicalIndicatorCriteriaValue | waarden die worden gebruikt bij de voorwaardelijke controle. |
| value2 | GraphicalIndicatorCriteriaValue | tweede waarde (einde van interval) die wordt gebruikt bij de voorwaardelijke controle in het geval van 'IsWithin' en 'IsNotWithing'-condities. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentException | Wordt gegooid wanneer een onjuiste combinatie van argumenten aan de constructor wordt doorgegeven. |

### Zie ook

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Initialiseert een nieuw exemplaar van het [`GraphicalIndicatorCriteria`](../) type.

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | waarde van de [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) enum die aangeeft op welke rijen de indicator wordt toegepast. |
| test | FilterComparisonType | waarde van de [`FilterComparisonType`](../../filtercomparisontype/) die het type vergelijking aangeeft dat door de criteria wordt uitgevoerd. |
| imageIndex | Int32 | de index van de afbeelding die moet worden weergegeven wanneer het veld aan de criteria voldoet. |
| value | GraphicalIndicatorCriteriaValue | waarde die wordt gebruikt bij de voorwaardelijke controle. |

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentException | Wordt gegooid wanneer een onjuiste combinatie van argumenten aan de constructor wordt doorgegeven. |
| ArgumentException | Wanneer de waarde van IsWithin of IsNotWithing wordt doorgegeven aan het testargument. |

### Zie ook

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


