---
title: "GroupCriterion"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά ένα κριτήριο σε έναν ορισμό ομάδας."
type: docs
weight: 124
url: /el/java/com.aspose.tasks/groupcriterion/
---

**Inheritance:**
java.lang.Object
```
public class GroupCriterion
```

Αντιπροσωπεύει ένα κριτήριο σε έναν ορισμό ομάδας. Το αντικείμενο GroupCriterion είναι μέλος της συλλογής [GroupCriterionCollection](../../com.aspose.tasks/groupcriterioncollection).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GroupCriterion()](#GroupCriterion--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [getAscending()](#getAscending--) | Επιστρέφει μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας είναι ταξινομημένο σε αύξουσα σειρά. |
| [getCellColor()](#getCellColor--) | Επιστρέφει το χρώμα του φόντου του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [getField()](#getField--) | Επιστρέφει το πεδίο με το οποίο γίνεται ομαδοποίηση. |
| [getFont()](#getFont--) | Επιστρέφει τη γραμματοσειρά για ένα κριτήριο σε έναν ορισμό ομάδας. |
| [getFontColor()](#getFontColor--) | Επιστρέφει το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [getGroupInterval()](#getGroupInterval--) | Επιστρέφει το διάστημα για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [getGroupOn()](#getGroupOn--) | Επιστρέφει τον τύπο ομαδοποίησης για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [getPattern()](#getPattern--) | Επιστρέφει το μοτίβο του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [getStartAt()](#getStartAt--) | Επιστρέφει την αρχή των διαστημάτων για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [hashCode()](#hashCode--) | Λειτουργεί ως συνάρτηση κατακερματισμού για έναν συγκεκριμένο τύπο. |
| [setAscending(boolean value)](#setAscending-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας ταξινομείται σε αύξουσα σειρά. |
| [setCellColor(Color value)](#setCellColor-java.awt.Color-) | Ορίζει το χρώμα του φόντου του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [setField(int value)](#setField-int-) | Ορίζει το πεδίο με το οποίο γίνεται ομαδοποίηση. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Ορίζει τη γραμματοσειρά για ένα κριτήριο σε έναν ορισμό ομάδας. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Ορίζει το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [setGroupInterval(Object value)](#setGroupInterval-java.lang.Object-) | Ορίζει το διάστημα για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [setGroupOn(int value)](#setGroupOn-int-) | Ορίζει τον τύπο ομαδοποίησης για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [setPattern(int value)](#setPattern-int-) | Ορίζει το μοτίβο του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
| [setStartAt(Object value)](#setStartAt-java.lang.Object-) | Ορίζει την έναρξη των διαστημάτων για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |
### GroupCriterion() {#GroupCriterion--}
```
public GroupCriterion()
```


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
boolean - **True** εάν το o είναι ένα GroupCriterion που έχει την ίδια τιμή UID με αυτήν την παρουσία· διαφορετικά, **false**.
### getAscending() {#getAscending--}
```
public final boolean getAscending()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας ταξινομείται σε αύξουσα σειρά. False εάν το πεδίο ταξινομείται σε φθίνουσα σειρά.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας ταξινομείται σε αύξουσα σειρά.
### getCellColor() {#getCellColor--}
```
public final Color getCellColor()
```


Επιστρέφει το χρώμα του φόντου του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Returns:**
java.awt.Color - το χρώμα του φόντου του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.
### getField() {#getField--}
```
public final int getField()
```


Επιστρέφει το πεδίο με το οποίο γίνεται ομαδοποίηση.

**Returns:**
int - το πεδίο με το οποίο γίνεται ομαδοποίηση.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Επιστρέφει τη γραμματοσειρά για ένα κριτήριο σε έναν ορισμό ομάδας.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font for a criterion in a group definition.
### getFontColor() {#getFontColor--}
```
public final Color getFontColor()
```


Επιστρέφει το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Returns:**
java.awt.Color - το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.
### getGroupInterval() {#getGroupInterval--}
```
public final Object getGroupInterval()
```


Επιστρέφει το διάστημα για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Returns:**
java.lang.Object - το διάστημα για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.
### getGroupOn() {#getGroupOn--}
```
public final int getGroupOn()
```


Επιστρέφει τον τύπο ομαδοποίησης για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Returns:**
int - ο τύπος ομαδοποίησης για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.
### getPattern() {#getPattern--}
```
public final int getPattern()
```


Επιστρέφει το μοτίβο του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Returns:**
int - το μοτίβο του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.
### getStartAt() {#getStartAt--}
```
public final Object getStartAt()
```


Επιστρέφει την αρχή των διαστημάτων για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Returns:**
java.lang.Object - η έναρξη των διαστημάτων για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Λειτουργεί ως συνάρτηση κατακερματισμού για έναν συγκεκριμένο τύπο.

**Returns:**
int - Ένας κωδικός κατακερματισμού για το τρέχον Object.
### setAscending(boolean value) {#setAscending-boolean-}
```
public final void setAscending(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας ταξινομείται σε αύξουσα σειρά. False εάν το πεδίο ταξινομείται σε φθίνουσα σειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας ταξινομείται σε αύξουσα σειρά. |

### setCellColor(Color value) {#setCellColor-java.awt.Color-}
```
public final void setCellColor(Color value)
```


Ορίζει το χρώμα του φόντου του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | το χρώμα του φόντου του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας. |

### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Ορίζει το πεδίο με το οποίο γίνεται ομαδοποίηση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το πεδίο με το οποίο γίνεται ομαδοποίηση. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Ορίζει τη γραμματοσειρά για ένα κριτήριο σε έναν ορισμό ομάδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | η γραμματοσειρά για ένα κριτήριο σε ορισμό ομάδας. |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public final void setFontColor(Color value)
```


Ορίζει το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |

### setGroupInterval(Object value) {#setGroupInterval-java.lang.Object-}
```
public final void setGroupInterval(Object value)
```


Ορίζει το διάστημα για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Object | το διάστημα για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |

### setGroupOn(int value) {#setGroupOn-int-}
```
public final void setGroupOn(int value)
```


Ορίζει τον τύπο ομαδοποίησης για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τύπος ομαδοποίησης για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |

### setPattern(int value) {#setPattern-int-}
```
public final void setPattern(int value)
```


Ορίζει το μοτίβο του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το μοτίβο του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |

### setStartAt(Object value) {#setStartAt-java.lang.Object-}
```
public final void setStartAt(Object value)
```


Ορίζει την έναρξη των διαστημάτων για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Object | η έναρξη των διαστημάτων για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |

