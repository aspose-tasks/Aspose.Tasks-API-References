---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "GraphicalIndicatorCriteria-Konstruktor. Initialisiert eine neue Instanz des Typs GraphicalIndicatorCriteria"
type: docs
weight: 10
url: /de/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Initialisiert eine neue Instanz des Typs [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | Wert des [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/)-Enums, der angibt, für welche Zeilen der Indikator angewendet wird |
| test | FilterComparisonType | Wert des [`FilterComparisonType`](../../filtercomparisontype/)-Enums, der den von den Kriterien durchgeführten Vergleichstyp bezeichnet. |
| imageIndex | Int32 | der Index des Bildes, das angezeigt wird, wenn das Feld die Kriterien erfüllt |
| value1 | GraphicalIndicatorCriteriaValue | Werte, die bei der Bedingungsprüfung verwendet werden. |
| value2 | GraphicalIndicatorCriteriaValue | zweiter Wert (Ende des Intervalls), der bei der Bedingungsprüfung im Fall der 'IsWithin'- und 'IsNotWithing'-Bedingungen verwendet wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Wird ausgelöst, wenn eine falsche Kombination von Argumenten an den Konstruktor übergeben wird. |

### Siehe auch

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Initialisiert eine neue Instanz des Typs [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | Wert des [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/)-Enums, der angibt, für welche Zeilen der Indikator angewendet wird |
| test | FilterComparisonType | Wert des [`FilterComparisonType`](../../filtercomparisontype/)-Enums, der den von den Kriterien durchgeführten Vergleichstyp bezeichnet. |
| imageIndex | Int32 | der Index des Bildes, das angezeigt wird, wenn das Feld die Kriterien erfüllt |
| Wert | GraphicalIndicatorCriteriaValue | Wert, der bei der Bedingungsprüfung verwendet wird. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Wird ausgelöst, wenn eine falsche Kombination von Argumenten an den Konstruktor übergeben wird. |
| ArgumentException | Wenn der Wert von IsWithin oder IsNotWithing an das Testargument übergeben wird. |

### Siehe auch

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


