---
title: "GraphicalIndicatorCriteria"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά ένα κριτήριο γραφικού δείκτη που συνδέεται με μια εκτεταμένη ιδιότητα."
type: docs
weight: 115
url: /el/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Αναπαριστά ένα κριτήριο γραφικού δείκτη που συνδέεται με μια εκτεταμένη ιδιότητα.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Αρχικοποιεί μια νέα παρουσία του τύπου [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Αρχικοποιεί μια νέα παρουσία του τύπου [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Λαμβάνει τον δείκτη της εικόνας που θα εμφανιστεί όταν το πεδίο ικανοποιεί τα κριτήρια. |
| [getRowType()](#getRowType--) | Λαμβάνει την τιμή του enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης. |
| [getTest()](#getTest--) | Λαμβάνει τον τύπο σύγκρισης που γίνεται μεταξύ της τιμής του εκτεταμένου χαρακτηριστικού και των τιμών που λειτουργούν ως κριτήριο για την εφαρμογή του γραφικού δείκτη. |
| [getValue1()](#getValue1--) | Λαμβάνει την τιμή που χρησιμοποιείται για τη δοκιμή της τιμής του εκτεταμένου χαρακτηριστικού. |
| [getValue2()](#getValue2--) | Λαμβάνει τη δεύτερη τιμή που χρησιμοποιείται για τη δοκιμή της τιμής του εκτεταμένου χαρακτηριστικού σε περίπτωση τύπων σύγκρισης 'IsWithin' και 'IsNotWithin'. |
| [toString()](#toString--) | Επιστρέφει την αναπαράσταση συμβολοσειράς της παρουσίας της κλάσης [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria). |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Αρχικοποιεί μια νέα παρουσία του τύπου [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| rowType | int | τιμή του enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης |
| test | int | τιμή του [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype) που υποδεικνύει τον τύπο σύγκρισης που εκτελείται από το κριτήριο. |
| imageIndex | int | ο δείκτης της εικόνας που θα εμφανιστεί όταν το πεδίο ικανοποιεί τα κριτήρια |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | τιμές που χρησιμοποιούνται στον έλεγχο της συνθήκης. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | δεύτερη τιμή (τέλος διαστήματος) που χρησιμοποιείται στον έλεγχο της συνθήκης σε περίπτωση συνθηκών 'IsWithin' και 'IsNotWithing'. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Αρχικοποιεί μια νέα παρουσία του τύπου [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| rowType | int | τιμή του enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης |
| test | int | τιμή του [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype) που υποδεικνύει τον τύπο σύγκρισης που εκτελείται από το κριτήριο. |
| imageIndex | int | ο δείκτης της εικόνας που θα εμφανιστεί όταν το πεδίο ικανοποιεί τα κριτήρια |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | τιμή που χρησιμοποιείται στον έλεγχο της συνθήκης. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Λαμβάνει τον δείκτη της εικόνας που θα εμφανιστεί όταν το πεδίο ικανοποιεί τα κριτήρια.

**Returns:**
int - ο δείκτης της εικόνας που θα εμφανιστεί όταν το πεδίο ικανοποιεί τα κριτήρια.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Λαμβάνει την τιμή του enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης.

**Returns:**
int - η τιμή του enum [GraphicalIndicatorCriteriaType](../../com.aspose/tasks/graphicalindicatorcriteriatype) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης.
### getTest() {#getTest--}
```
public final int getTest()
```


Λαμβάνει τον τύπο σύγκρισης που γίνεται μεταξύ της τιμής του εκτεταμένου χαρακτηριστικού και των τιμών που λειτουργούν ως κριτήριο για την εφαρμογή του γραφικού δείκτη. [FilterComparisonType](../../com.aspose/tasks/filtercomparisontype)

**Returns:**
int - ο τύπος σύγκρισης που γίνεται μεταξύ της τιμής του εκτεταμένου χαρακτηριστικού και των τιμών που λειτουργούν ως κριτήριο για την εφαρμογή του γραφικού δείκτη.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Λαμβάνει την τιμή που χρησιμοποιείται για τη δοκιμή της τιμής του εκτεταμένου χαρακτηριστικού.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Λαμβάνει τη δεύτερη τιμή που χρησιμοποιείται για τη δοκιμή της τιμής του εκτεταμένου χαρακτηριστικού σε περίπτωση τύπων σύγκρισης 'IsWithin' και 'IsNotWithin'.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Επιστρέφει την αναπαράσταση συμβολοσειράς της παρουσίας της κλάσης [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria).

**Returns:**
java.lang.String - αναπαράσταση συμβολοσειράς αυτού του αντικειμένου.
