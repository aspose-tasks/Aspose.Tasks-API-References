---
title: "Filter"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά ένα φίλτρο στο Project."
type: docs
weight: 91
url: /el/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Αναπαριστά ένα φίλτρο στο Project.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Filter()](#Filter--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Συγκρίνει αυτή την παρουσία με την καθορισμένη παρουσία της κλάσης [Filter](../../com.aspose.tasks/filter) και επιστρέφει μια ένδειξη της σχετικής τους σειράς. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline. |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline. |
| [getCriteria()](#getCriteria--) | Λαμβάνει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP. |
| [getFilterType()](#getFilterType--) | Λαμβάνει τον τύπο του φίλτρου. |
| [getIndex()](#getIndex--) | Λαμβάνει το δείκτη ενός αντικειμένου [Filter](../../com.aspose.tasks/filter) στο αντικείμενο που περιέχει τα Filters. |
| [getName()](#getName--) | Λαμβάνει το όνομα ενός αντικειμένου Filter. |
| [getShowInMenu()](#getShowInMenu--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το έργο εμφανίζει το όνομα του φίλτρου στη λίστα επιλογής Filter στην καρτέλα Προβολή της κορδέλας. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Λαμβάνει μια τιμή που υποδεικνύει εάν εμφανίζονται σχετικές γραμμές σύνοψης για το φίλτρο. |
| [getUid()](#getUid--) | Λαμβάνει το μοναδικό αναγνωριστικό ενός φίλτρου. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το φίλτρο. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Ορίζει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP. |
| [setFilterType(int value)](#setFilterType-int-) | Ο τύπος του φίλτρου. |
| [setName(String value)](#setName-java.lang.String-) | Ορίζει το όνομα ενός αντικειμένου Filter. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το έργο εμφανίζει το όνομα του φίλτρου στη λίστα επιλογής Filter στην καρτέλα Προβολή της κορδέλας. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν εμφανίζονται σχετικές γραμμές σύνοψης για το φίλτρο. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Συγκρίνει αυτή την παρουσία με την καθορισμένη παρουσία της κλάσης [Filter](../../com.aspose.tasks/filter) και επιστρέφει μια ένδειξη της σχετικής τους σειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | την καθορισμένη παρουσία της κλάσης [Filter](../../com.aspose.tasks/filter) για σύγκριση με αυτό το αντικείμενο. |

**Returns:**
int - ένδειξη της σχετικής τους σειράς.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | το καθορισμένο αντικείμενο AssignmentBaseline για σύγκριση με αυτή την παρουσία. |

**Returns:**
boolean - επιστρέφει true εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline· διαφορετικά, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | το καθορισμένο αντικείμενο AssignmentBaseline για σύγκριση με αυτή την παρουσία. |

**Returns:**
boolean - επιστρέφει true εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο AssignmentBaseline· διαφορετικά, false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Λαμβάνει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Λαμβάνει τον τύπο του φίλτρου.

**Returns:**
int - ο τύπος του φίλτρου.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Λαμβάνει το δείκτη ενός αντικειμένου [Filter](../../com.aspose.tasks/filter) στο αντικείμενο που περιέχει τα Filters.

**Returns:**
int - ο δείκτης ενός αντικειμένου [Filter](../../com.aspose.tasks/filter) στο αντικείμενο που περιέχει τα Filters.
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει το όνομα ενός αντικειμένου Filter.

**Returns:**
java.lang.String - το όνομα ενός αντικειμένου Filter.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το έργο εμφανίζει το όνομα του φίλτρου στη λίστα επιλογής Filter στην καρτέλα Προβολή της κορδέλας.

**Returns:**
boolean - τιμή που υποδεικνύει εάν το έργο εμφανίζει το όνομα του φίλτρου στη λίστα αναπτυσσόμενου Φίλτρου στην καρτέλα Προβολή της κορδέλας.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν εμφανίζονται σχετικές γραμμές σύνοψης για το φίλτρο.

**Returns:**
boolean - τιμή που υποδεικνύει εάν εμφανίζονται σχετικές γραμμές σύνοψης για το φίλτρο.
### getUid() {#getUid--}
```
public final int getUid()
```


Λαμβάνει το μοναδικό αναγνωριστικό ενός φίλτρου.

**Returns:**
int - το μοναδικό αναγνωριστικό ενός φίλτρου.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για το φίλτρο.

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Το πρώτο φίλτρο. |
| b | [Filter](../../com.aspose.tasks/filter) | Το δεύτερο φίλτρο. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Το πρώτο φίλτρο. |
| b | [Filter](../../com.aspose.tasks/filter) | Το δεύτερο φίλτρο. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Το πρώτο φίλτρο. |
| b | [Filter](../../com.aspose.tasks/filter) | Το δεύτερο φίλτρο. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Το πρώτο φίλτρο. |
| b | [Filter](../../com.aspose.tasks/filter) | Το δεύτερο φίλτρο. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Το πρώτο φίλτρο. |
| b | [Filter](../../com.aspose.tasks/filter) | Το δεύτερο φίλτρο. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Το πρώτο φίλτρο. |
| b | [Filter](../../com.aspose.tasks/filter) | Το δεύτερο φίλτρο. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Ορίζει τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | τα κριτήρια που πρέπει να πληρούν οι εργασίες ή οι πόροι για να εμφανιστούν στην προβολή MSP. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


Ο τύπος του φίλτρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τύπος του φίλτρου. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ορίζει το όνομα ενός αντικειμένου Filter.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το όνομα ενός αντικειμένου Filter. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το έργο εμφανίζει το όνομα του φίλτρου στη λίστα επιλογής Filter στην καρτέλα Προβολή της κορδέλας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν το έργο εμφανίζει το όνομα του φίλτρου στη λίστα αναπτυσσόμενου Φίλτρου στην καρτέλα Προβολή της κορδέλας. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν εμφανίζονται σχετικές γραμμές σύνοψης για το φίλτρο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν εμφανίζονται σχετικές γραμμές σύνοψης για το φίλτρο. |

