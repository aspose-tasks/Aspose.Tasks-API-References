---
title: "View"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια προβολή στο Project."
type: docs
weight: 342
url: /el/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Αναπαριστά μια προβολή στο Project.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [View()](#View--) | Αρχικοποιεί μια νέα περίπτωση της κλάσης [View](../../com.aspose/tasks/view). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Συγκρίνει την τρέχουσα περίπτωση με ένα άλλο αντικείμενο του ίδιου τύπου και επιστρέφει έναν ακέραιο που υποδεικνύει εάν η τρέχουσα περίπτωση προηγείται, ακολουθεί ή βρίσκεται στην ίδια θέση στη σειρά ταξινόμησης με το άλλο αντικείμενο. |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Δημιουργεί μια νέα περίπτωση της κλάσης [View](../../com.aspose/tasks/view). |
| [getFilter()](#getFilter--) | Λαμβάνει ένα φίλτρο που χρησιμοποιείται σε μια μοναδική προβολή. |
| [getGroup()](#getGroup--) | Λαμβάνει μια ομάδα της μοναδικής προβολής. |
| [getHighlightFilter()](#getHighlightFilter--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια μοναδική προβολή. |
| [getName()](#getName--) | Λαμβάνει το όνομα ενός αντικειμένου View. |
| [getPageInfo()](#getPageInfo--) | Λαμβάνει μια περίπτωση της κλάσης `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). |
| [getParentProject()](#getParentProject--) | Λαμβάνει το γονικό αντικείμενο του View. |
| [getScreen()](#getScreen--) | Λαμβάνει τον τύπο οθόνης για τη μοναδική προβολή. |
| [getShowInMenu()](#getShowInMenu--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της μοναδικής προβολής στη λίστα επιλογής View ή Other Views στη λωρίδα εργαλείων. |
| [getTable()](#getTable--) | Λαμβάνει έναν πίνακα της μοναδικής προβολής. |
| [getType()](#getType--) | Λαμβάνει τον τύπο του στοιχείου στην ενιαία προβολή, όπως εργασίες ή πόρους. |
| [getUid()](#getUid--) | Λαμβάνει το μοναδικό αναγνωριστικό μιας προβολής. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Λαμβάνει μια συλλογή αντικειμένων που αντιπροσωπεύουν τη θέση και την εμφάνιση του [OleObject](../../com.aspose.tasks/oleobject) στην προβολή. |
| [hashCode()](#hashCode--) | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το στιγμιότυπο της κλάσης [Resource](../../com.aspose.tasks/resource). |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Ορίζει ένα φίλτρο που χρησιμοποιείται σε μια ενιαία προβολή. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Ορίζει μια ομάδα της ενιαίας προβολής. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια ενιαία προβολή. |
| [setName(String value)](#setName-java.lang.String-) | Ορίζει το όνομα ενός αντικειμένου View. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της ενιαίας προβολής στις λίστες αναπτυσσόμενων επιλογών View ή Other Views στη λωρίδα. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Ορίζει έναν πίνακα της ενιαίας προβολής. |
### View() {#View--}
```
public View()
```


Αρχικοποιεί μια νέα περίπτωση της κλάσης [View](../../com.aspose/tasks/view).

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Συγκρίνει την τρέχουσα περίπτωση με ένα άλλο αντικείμενο του ίδιου τύπου και επιστρέφει έναν ακέραιο που υποδεικνύει εάν η τρέχουσα περίπτωση προηγείται, ακολουθεί ή βρίσκεται στην ίδια θέση στη σειρά ταξινόμησης με το άλλο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | το καθορισμένο αντικείμενο View για σύγκριση με αυτήν την παρουσία. |

**Returns:**
int - Ένας 32-bit υπογεγραμμένος ακέραιος που υποδεικνύει τη σχετική σειρά των αντικειμένων που συγκρίνονται. Η τιμή επιστροφής έχει τις ακόλουθες σημασίες: Τιμή Σημασία Μικρότερη του μηδενός Αυτό το αντικείμενο προηγείται του `other` στη σειρά ταξινόμησης. Μηδέν Αυτό το αντικείμενο βρίσκεται στην ίδια θέση στη σειρά ταξινόμησης με το `other`. Μεγαλύτερη του μηδενός Αυτό το αντικείμενο ακολουθεί το `other` στη σειρά ταξινόμησης.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

**Returns:**
boolean - **True** εάν το καθορισμένο αντικείμενο είναι ένα View που έχει την ίδια τιμή Uid με αυτήν την παρουσία· διαφορετικά, **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Δημιουργεί μια νέα περίπτωση της κλάσης [View](../../com.aspose/tasks/view).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| viewScreen | int | Ο τύπος οθόνης για τον οποίο μπορεί να εμφανιστεί η προβολή. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Λαμβάνει ένα φίλτρο που χρησιμοποιείται σε μια μοναδική προβολή.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Λαμβάνει μια ομάδα της μοναδικής προβολής.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια μοναδική προβολή.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια ενιαία προβολή.
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει το όνομα ενός αντικειμένου View.

**Returns:**
java.lang.String - το όνομα ενός αντικειμένου View.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Λαμβάνει μια παρουσία της κλάσης `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). Αντιπροσωπεύει τα δεδομένα ρύθμισης σελίδας που υπάρχουν σε μορφή αρχείου mpp.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Λαμβάνει το γονικό αντικείμενο του View. Μόνο για ανάγνωση [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Λαμβάνει τον τύπο οθόνης για την ενιαία προβολή. Μόνο για ανάγνωση [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - ο τύπος οθόνης για την ενιαία προβολή.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της μοναδικής προβολής στη λίστα επιλογής View ή Other Views στη λωρίδα εργαλείων.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της ενιαίας προβολής στις λίστες αναπτυσσόμενων επιλογών View ή Other Views στη λωρίδα.
### getTable() {#getTable--}
```
public final Table getTable()
```


Λαμβάνει έναν πίνακα της μοναδικής προβολής.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Λαμβάνει τον τύπο του στοιχείου στην ενιαία προβολή, όπως εργασίες ή πόρους. Μόνο για ανάγνωση [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - ο τύπος του στοιχείου στην ενιαία προβολή, όπως εργασίες ή πόρους.
### getUid() {#getUid--}
```
public final int getUid()
```


Λαμβάνει το μοναδικό αναγνωριστικό μιας προβολής.

**Returns:**
int - το μοναδικό αναγνωριστικό μιας προβολής.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Λαμβάνει μια συλλογή αντικειμένων που αντιπροσωπεύουν τη θέση και την εμφάνιση του [OleObject](../../com.aspose.tasks/oleobject) στην προβολή.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - μια συλλογή αντικειμένων που αντιπροσωπεύει τη θέση και την εμφάνιση του [OleObject](../../com.aspose.tasks/oleobject) στην προβολή.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Επιστρέφει μια τιμή κώδικα κατακερματισμού για το στιγμιότυπο της κλάσης [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Η πρώτη προβολή. |
| b | [View](../../com.aspose.tasks/view) | Η δεύτερη προβολή. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Η πρώτη προβολή. |
| b | [View](../../com.aspose.tasks/view) | Η δεύτερη προβολή. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη από ένα καθορισμένο αντικείμενο
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Η πρώτη προβολή. |
| b | [View](../../com.aspose.tasks/view) | Η δεύτερη προβολή. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μεγαλύτερη ή ίση με ένα καθορισμένο αντικείμενο
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Η πρώτη προβολή. |
| b | [View](../../com.aspose.tasks/view) | Η δεύτερη προβολή. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Το πρώτο φίλτρο. |
| b | [View](../../com.aspose.tasks/view) | Το δεύτερο φίλτρο. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη από ένα καθορισμένο αντικείμενο
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Η πρώτη προβολή. |
| b | [View](../../com.aspose.tasks/view) | Η δεύτερη προβολή. |

**Returns:**
boolean - τιμή που υποδεικνύει εάν αυτή η παρουσία είναι μικρότερη ή ίση με ένα καθορισμένο αντικείμενο
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Ορίζει ένα φίλτρο που χρησιμοποιείται σε μια ενιαία προβολή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | ένα φίλτρο που χρησιμοποιείται σε μια μοναδική προβολή. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Ορίζει μια ομάδα της ενιαίας προβολής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | μια ομάδα της μοναδικής προβολής. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια ενιαία προβολή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια μοναδική προβολή. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ορίζει το όνομα ενός αντικειμένου View.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το όνομα ενός αντικειμένου View. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της ενιαίας προβολής στις λίστες αναπτυσσόμενων επιλογών View ή Other Views στη λωρίδα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της μοναδικής προβολής στη λίστα View ή Other Views στο Ribbon. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Ορίζει έναν πίνακα της ενιαίας προβολής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | ένας πίνακας της μοναδικής προβολής. |

