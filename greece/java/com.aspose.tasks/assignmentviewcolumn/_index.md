---
title: "AssignmentViewColumn"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Κλάση προβολής έργων."
type: docs
weight: 19
url: /el/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Κλάση προβολής του έργου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης AssignmentViewColumn. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Μετατρέπει την τρέχουσα ανάθεση πόρου σε κείμενο στήλης. |
| [getField()](#getField--) | Επιστρέφει το πεδίο της στήλης. |
| [setField(int value)](#setField-int-) | Ορίζει το πεδίο της στήλης. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης AssignmentViewColumn.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Όνομα στήλης. |
| width | int | Πλάτος στήλης σε εικονοστοιχεία. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Μετατροπέας δεδομένων ανάθεσης σε κείμενο στήλης. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Μετατρέπει την τρέχουσα ανάθεση πόρου σε κείμενο στήλης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Τρέχουσα ανάθεση. |

**Returns:**
java.lang.String - Το κείμενο της στήλης.
### getField() {#getField--}
```
public int getField()
```


Επιστρέφει το πεδίο της στήλης. `Field`.

**Returns:**
int - τιμή πεδίου στήλης.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Ορίζει το πεδίο της στήλης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | τιμή πεδίου στήλης. |

