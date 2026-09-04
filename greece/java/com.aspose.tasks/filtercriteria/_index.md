---
title: "FilterCriteria"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Ορίζει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP."
type: docs
weight: 94
url: /el/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Ορίζει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Λαμβάνει τη λίστα των θυγατρικών γραμμών [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
| [getField()](#getField--) | Λαμβάνει ένα `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) για αλλαγή. |
| [getOperation()](#getOperation--) | Λαμβάνει το κριτήριο που καθορίζεται με τα FieldName, Test και Value και σχετίζεται με άλλα κριτήρια στο φίλτρο. |
| [getTest()](#getTest--) | Λαμβάνει τον τύπο σύγκρισης που γίνεται μεταξύ FieldName και Value και λειτουργεί ως κριτήριο επιλογής για το φίλτρο. |
| [getValues()](#getValues--) | Λαμβάνει τις τιμές αντικειμένων για σύγκριση με την τιμή του πεδίου που καθορίζεται με το FieldName. |
| [isValueAField()](#isValueAField--) | Λαμβάνει αν η δεξιά τιμή του FilterCriteria είναι αναφορά πεδίου, όχι σταθερή τιμή. |
| [isValueAField(int index)](#isValueAField-int-) | Λαμβάνει αν η τιμή στο δείκτη του FilterCriteria είναι αναφορά πεδίου, όχι σταθερή τιμή. |
| [setField(int value)](#setField-int-) | Ορίζει ένα `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) για αλλαγή. |
| [setOperation(int value)](#setOperation-int-) | Ορίζει το κριτήριο που καθορίζεται με τα FieldName, Test και Value και σχετίζεται με άλλα κριτήρια στο φίλτρο. |
| [setTest(int value)](#setTest-int-) | Ορίζει τον τύπο σύγκρισης που γίνεται μεταξύ FieldName και Value και λειτουργεί ως κριτήριο επιλογής για το φίλτρο. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | Ορίζει την τιμή αντικειμένου στο δείκτη για σύγκριση με την τιμή του πεδίου που καθορίζεται από το FieldName. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Ορίζει την τιμή αντικειμένου για σύγκριση με την τιμή του πεδίου που καθορίζεται από το FieldName. |
| [setValueByField(int value)](#setValueByField-int-) | Ορίζει το πεδίο του οποίου η τιμή θα συγκριθεί με την τιμή του πεδίου που καθορίζεται από το FieldName. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | Ορίζει το πεδίο στο δείκτη του οποίου η τιμή θα συγκριθεί με την τιμή του πεδίου που καθορίζεται από το FieldName. |
| [toString()](#toString--) | Επιστρέφει την αναπαράσταση σε μορφή συμβολοσειράς της παρουσίας της κλάσης [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Λαμβάνει τη λίστα των θυγατρικών γραμμών [FilterCriteria](../../com.aspose.tasks/filtercriteria). Εάν το φίλτρο περιέχει περισσότερες από μία γραμμές κριτηρίων, τότε η επίδραση του τελεστή And είναι ότι τα κριτήρια και για τις δύο γραμμές πρέπει να ικανοποιηθούν ώστε η εργασία ή ο πόρος να εμφανιστούν ως αποτέλεσμα αυτού του φίλτρου. Η επίδραση του τελεστή Or είναι ότι τα κριτήρια για τη μία ή την άλλη γραμμή πρέπει να ικανοποιηθούν.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - η λίστα των θυγατρικών γραμμών [FilterCriteria](../../com.aspose.tasks/filtercriteria) rows.
### getField() {#getField--}
```
public final int getField()
```


Λαμβάνει ένα `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) για αλλαγή.

**Returns:**
int - ένα `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) για αλλαγή.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Λαμβάνει το κριτήριο που καθορίζεται με τα FieldName, Test και Value και σχετίζεται με άλλα κριτήρια στο φίλτρο.

**Returns:**
int - το κριτήριο που καθορίζεται με τα FieldName, Test και Value και σχετίζεται με άλλα κριτήρια στο φίλτρο.
### getTest() {#getTest--}
```
public final int getTest()
```


Λαμβάνει τον τύπο σύγκρισης που γίνεται μεταξύ FieldName και Value και λειτουργεί ως κριτήριο επιλογής για το φίλτρο. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - ο τύπος σύγκρισης που γίνεται μεταξύ FieldName και Value και λειτουργεί ως κριτήριο επιλογής για το φίλτρο.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


Λαμβάνει τις τιμές αντικειμένων για σύγκριση με την τιμή του πεδίου που καθορίζεται με το FieldName.

**Returns:**
java.lang.Object[] - οι τιμές αντικειμένων για σύγκριση με την τιμή του πεδίου που καθορίζεται με το FieldName.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


Λαμβάνει αν η δεξιά τιμή του FilterCriteria είναι αναφορά πεδίου, όχι σταθερή τιμή.

**Returns:**
boolean - αν η δεξιά τιμή του FilterCriteria είναι αναφορά πεδίου, όχι σταθερή τιμή.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


Λαμβάνει αν η τιμή στο δείκτη του FilterCriteria είναι αναφορά πεδίου, όχι σταθερή τιμή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | ο δείκτης της τιμής |

**Returns:**
boolean - εάν η τιμή στα δεξιά στο δείκτη του FilterCriteria είναι αναφορά πεδίου, όχι σταθερή τιμή.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Ορίζει ένα `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) για αλλαγή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | ένα `Field`([getField()](../../com.aspose/tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) για αλλαγή. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Ορίζει το κριτήριο που καθορίζεται με τα FieldName, Test και Value και σχετίζεται με άλλα κριτήρια στο φίλτρο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το κριτήριο που καθορίζεται με το FieldName, Test και Value σχετίζεται με άλλα κριτήρια στο φίλτρο. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Ορίζει τον τύπο σύγκρισης μεταξύ του FieldName και του Value που λειτουργεί ως κριτήριο επιλογής για το φίλτρο. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τύπος σύγκρισης μεταξύ του FieldName και του Value που λειτουργεί ως κριτήριο επιλογής για το φίλτρο. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


Ορίζει την τιμή αντικειμένου στο δείκτη για σύγκριση με την τιμή του πεδίου που καθορίζεται από το FieldName.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | ο δείκτης της τιμής. |
| τιμή | java.lang.Object | τιμή αντικειμένου που θα χρησιμεύσει ως τιμή στα δεξιά στο δείκτη του κριτηρίου φίλτρου. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


Ορίζει την τιμή αντικειμένου για σύγκριση με την τιμή του πεδίου που καθορίζεται από το FieldName.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Object | τιμή αντικειμένου που θα χρησιμεύσει ως τιμή στα δεξιά του κριτηρίου φίλτρου. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


Ορίζει το πεδίο του οποίου η τιμή θα συγκριθεί με την τιμή του πεδίου που καθορίζεται από το FieldName.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Πεδίο που θα χρησιμεύσει ως τιμή στα δεξιά του κριτηρίου φίλτρου. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


Ορίζει το πεδίο στο δείκτη του οποίου η τιμή θα συγκριθεί με την τιμή του πεδίου που καθορίζεται από το FieldName.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | ο δείκτης της τιμής |
| τιμή | int | Πεδίο που θα χρησιμεύσει ως τιμή στα δεξιά στο δείκτη του κριτηρίου φίλτρου. |

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει την αναπαράσταση σε μορφή συμβολοσειράς της παρουσίας της κλάσης [FilterCriteria](../../com.aspose.tasks/filtercriteria).

**Returns:**
java.lang.String - αναπαράσταση συμβολοσειράς αυτού του αντικειμένου.
