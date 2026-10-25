---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής GraphicalIndicatorCriteria. Αρχικοποιεί μια νέα παρουσία του τύπου GraphicalIndicatorCriteria"
type: docs
weight: 10
url: /el/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του τύπου [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | Τιμή του enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης |
| test | FilterComparisonType | Τιμή του [`FilterComparisonType`](../../filtercomparisontype/) που υποδεικνύει τον τύπο σύγκρισης που εκτελείται από το κριτήριο. |
| imageIndex | Int32 | ο δείκτης της εικόνας που θα εμφανιστεί όταν το πεδίο ικανοποιεί τα κριτήρια |
| value1 | GraphicalIndicatorCriteriaValue | τιμές που χρησιμοποιούνται στον έλεγχο συνθήκης. |
| value2 | GraphicalIndicatorCriteriaValue | δεύτερη τιμή (τέλος διαστήματος) που χρησιμοποιείται στον έλεγχο συνθήκης σε περίπτωση συνθηκών 'IsWithin' και 'IsNotWithing'. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Εγείρεται όταν περάσει λανθασμένος συνδυασμός ορισμάτων στον κατασκευαστή. |

### Δείτε επίσης

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Αρχικοποιεί μια νέα παρουσία του τύπου [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | Τιμή του enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης |
| test | FilterComparisonType | Τιμή του [`FilterComparisonType`](../../filtercomparisontype/) που υποδεικνύει τον τύπο σύγκρισης που εκτελείται από το κριτήριο. |
| imageIndex | Int32 | ο δείκτης της εικόνας που θα εμφανιστεί όταν το πεδίο ικανοποιεί τα κριτήρια |
| value | GraphicalIndicatorCriteriaValue | τιμή που χρησιμοποιείται στον έλεγχο συνθήκης. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Εγείρεται όταν περάσει λανθασμένος συνδυασμός ορισμάτων στον κατασκευαστή. |
| ArgumentException | Όταν η τιμή του IsWithin ή του IsNotWithing περνιέται ως όρισμα ελέγχου. |

### Δείτε επίσης

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


