---
title: "BarStyle"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αλλάξτε το οπτικό στυλ της γραμμής για το στοιχείο στην προβολή έργου."
type: docs
weight: 25
url: /el/java/com.aspose.tasks/barstyle/
---

**Inheritance:**
java.lang.Object
```
public class BarStyle
```

Αλλάξτε το οπτικό στυλ της γραμμής για το στοιχείο στην προβολή έργου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [BarStyle()](#BarStyle--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [BarStyle](../../com.aspose.tasks/barstyle). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBarColor()](#getBarColor--) | Λαμβάνει το java.awt.Color του στυλ ράβδου. |
| [getBarShape()](#getBarShape--) | Λαμβάνει το `BarShape`([getBarShape()](../../com.aspose.tasks/barstyle\#getBarShape--)/[setBarShape(int)](../../com.aspose.tasks/barstyle\#setBarShape-int-)) του στυλ ράβδου. |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στο κάτω μέρος της γραμμής της εργασίας. |
| [getBottomField()](#getBottomField--) | Λαμβάνει ένα πεδίο που θα εμφανίζεται στο κάτω μέρος της ράβδου. |
| [getEndShape()](#getEndShape--) | Λαμβάνει το [Shape](../../com.aspose.tasks/shape) στο τέλος της ράβδου. |
| [getEndShapeColor()](#getEndShapeColor--) | Λαμβάνει το java.awt.Color του σχήματος στο τέλος της ράβδου. |
| [getEndShapeType()](#getEndShapeType--) | Λαμβάνει τον τύπο του σχήματος τέλους. |
| [getFrom()](#getFrom--) | Λαμβάνει τη θέση του σημείου εκκίνησης της γραμμής gantt. |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί μέσα στη γραμμή της εργασίας. |
| [getInsideField()](#getInsideField--) | Λαμβάνει ένα πεδίο που θα εμφανίζεται μέσα στη ράβδο. |
| [getItemType()](#getItemType--) | Λαμβάνει το [BarItemType](../../com.aspose.tasks/baritemtype) του στυλ ράβδου. |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα αριστερά της γραμμής της εργασίας. |
| [getLeftField()](#getLeftField--) | Λαμβάνει ένα πεδίο που θα εμφανίζεται στα αριστερά της ράβδου. |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα δεξιά της μπάρας του έργου. |
| [getRightField()](#getRightField--) | Λαμβάνει ένα πεδίο που θα εμφανίζεται στα δεξιά της ράβδου. |
| [getStartShape()](#getStartShape--) | Λαμβάνει το [Shape](../../com.aspose.tasks/shape) στην αρχή της ράβδου. |
| [getStartShapeColor()](#getStartShapeColor--) | Λαμβάνει το java.awt.Color του σχήματος στην αρχή της ράβδου. |
| [getStartShapeType()](#getStartShapeType--) | Λαμβάνει έναν τύπο του αρχικού σχήματος. |
| [getTextStyle()](#getTextStyle--) | Λαμβάνει το στυλ του κειμένου της ράβδου. |
| [getTo()](#getTo--) | Λαμβάνει τη θέση του τελικού σημείου της μπάρας gantt. |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στην κορυφή της μπάρας του έργου. |
| [getTopField()](#getTopField--) | Λαμβάνει ένα πεδίο που θα εμφανίζεται στο πάνω μέρος της ράβδου. |
| [setBarColor(Color value)](#setBarColor-java.awt.Color-) | Ορίζει το java.awt.Color του στυλ ράβδου. |
| [setBarShape(int value)](#setBarShape-int-) | Ορίζει το `BarShape`([getBarShape()](../../com.aspose.tasks/barstyle\#getBarShape--)/[setBarShape(int)](../../com.aspose.tasks/barstyle\#setBarShape-int-)) του στυλ ράβδου. |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στο κάτω μέρος της μπάρας του έργου. |
| [setBottomField(int value)](#setBottomField-int-) | Ορίζει ένα πεδίο που θα εμφανίζεται στο κάτω μέρος της ράβδου. |
| [setEndShape(int value)](#setEndShape-int-) | Ορίζει το [Shape](../../com.aspose.tasks/shape) στο τέλος της ράβδου. |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | Ορίζει το java.awt.Color του σχήματος στο τέλος της ράβδου. |
| [setEndShapeType(int value)](#setEndShapeType-int-) | Ορίζει έναν τύπο του τελικού σχήματος. |
| [setFrom(int value)](#setFrom-int-) | Ορίζει τη θέση του αρχικού σημείου της μπάρας gantt. |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί μέσα στη μπάρα του έργου. |
| [setInsideField(int value)](#setInsideField-int-) | Ορίζει ένα πεδίο που θα εμφανίζεται μέσα στη ράβδο. |
| [setItemType(int value)](#setItemType-int-) | Ορίζει το [BarItemType](../../com.aspose.tasks/baritemtype) του στυλ ράβδου. |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα αριστερά της μπάρας του έργου. |
| [setLeftField(int value)](#setLeftField-int-) | Ορίζει ένα πεδίο που θα εμφανίζεται στα αριστερά της ράβδου. |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα δεξιά της μπάρας του έργου. |
| [setRightField(int value)](#setRightField-int-) | Ορίζει ένα πεδίο που θα εμφανίζεται στα δεξιά της μπάρας. |
| [setStartShape(int value)](#setStartShape-int-) | Ορίζει το [Shape](../../com.aspose.tasks/shape) στην αρχή της μπάρας. |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | Ορίζει το java.awt.Color του σχήματος στην αρχή της μπάρας. |
| [setStartShapeType(int value)](#setStartShapeType-int-) | Ορίζει έναν τύπο του αρχικού σχήματος. |
| [setTextStyle(TextStyle value)](#setTextStyle-com.aspose.tasks.TextStyle-) | Ορίζει το στυλ του κειμένου της μπάρας. |
| [setTo(int value)](#setTo-int-) | Ορίζει τη θέση του τελικού σημείου της μπάρας gantt. |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στην κορυφή της μπάρας του έργου. |
| [setTopField(int value)](#setTopField-int-) | Ορίζει ένα πεδίο που θα εμφανίζεται στην κορυφή της μπάρας. |
### BarStyle() {#BarStyle--}
```
public BarStyle()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [BarStyle](../../com.aspose.tasks/barstyle).

### getBarColor() {#getBarColor--}
```
public final Color getBarColor()
```


Λαμβάνει το java.awt.Color του στυλ ράβδου.

**Returns:**
java.awt.Color - ένα χρώμα του στυλ της μπάρας.
### getBarShape() {#getBarShape--}
```
public final int getBarShape()
```


Λαμβάνει το `BarShape`([getBarShape()](../../com.aspose.tasks/barstyle\#getBarShape--)/[setBarShape(int)](../../com.aspose.tasks/barstyle\#setBarShape-int-)) του στυλ ράβδου.

**Returns:**
int - [BarShape](../../com.aspose.tasks/barshape) του στυλ της μπάρας.
### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


Λαμβάνει τον μετατροπέα που ορίζεται από τον χρήστη για να λαμβάνει κείμενο που θα αποτυπώνεται στο κάτω μέρος της μπάρας της εργασίας. Αντικαθιστά την τιμή της `BottomField`([getBottomField()](../../com.aspose.tasks/barstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/barstyle\#setBottomField-int-)) ιδιότητας.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


Λαμβάνει ένα πεδίο που θα εμφανίζεται στο κάτω μέρος της ράβδου.

**Returns:**
int - ένα πεδίο που θα εμφανίζεται στο κάτω μέρος της μπάρας.
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


Λαμβάνει το [Shape](../../com.aspose.tasks/shape) στο τέλος της ράβδου.

**Returns:**
int - [Shape](../../com.aspose.tasks/shape) στο τέλος της μπάρας.
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


Λαμβάνει το java.awt.Color του σχήματος στο τέλος της ράβδου.

**Returns:**
java.awt.Color - ένα χρώμα του σχήματος στην αρχή της μπάρας.
### getEndShapeType() {#getEndShapeType--}
```
public final int getEndShapeType()
```


Λαμβάνει έναν τύπο του τελικού σχήματος. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Returns:**
int - ένας τύπος του τελικού σχήματος.
### getFrom() {#getFrom--}
```
public final int getFrom()
```


Λαμβάνει τη θέση του αρχικού σημείου της μπάρας gantt. [Field](../../com.aspose.tasks/field).

**Returns:**
int - μια θέση του αρχικού σημείου της μπάρας gantt.
### getInsideBarTextConverter() {#getInsideBarTextConverter--}
```
public final TaskBarTextConverter getInsideBarTextConverter()
```


Λαμβάνει τον μετατροπέα που ορίζεται από τον χρήστη για να λαμβάνει κείμενο που θα αποτυπώνεται μέσα στη μπάρα της εργασίας. Αντικαθιστά την τιμή της `InsideField`([getInsideField()](../../com.aspose.tasks/barstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/barstyle\#setInsideField-int-)) ιδιότητας.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


Λαμβάνει ένα πεδίο που θα εμφανίζεται μέσα στη ράβδο.

**Returns:**
int - ένα πεδίο που θα εμφανίζεται μέσα στη μπάρα.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Λαμβάνει το [BarItemType](../../com.aspose.tasks/baritemtype) του στυλ ράβδου.

**Returns:**
int - [BarItemType](../../com.aspose.tasks/baritemtype) του στυλ της μπάρας.
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


Λαμβάνει τον μετατροπέα που ορίζεται από τον χρήστη για να λαμβάνει κείμενο που θα αποτυπώνεται στα αριστερά της μπάρας της εργασίας. Αντικαθιστά την τιμή της `LeftField`([getLeftField()](../../com.aspose.tasks/barstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/barstyle\#setLeftField-int-)) ιδιότητας.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


Λαμβάνει ένα πεδίο που θα εμφανίζεται στα αριστερά της ράβδου.

**Returns:**
int - ένα πεδίο που θα εμφανίζεται στα αριστερά της μπάρας.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


Λαμβάνει τον μετατροπέα που ορίζεται από τον χρήστη για να λαμβάνει κείμενο που θα αποτυπώνεται στα δεξιά της μπάρας της εργασίας. Αντικαθιστά την τιμή της `RightField`([getRightField()](../../com.aspose.tasks/barstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/barstyle\#setRightField-int-)) ιδιότητας.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


Λαμβάνει ένα πεδίο που θα εμφανίζεται στα δεξιά της ράβδου.

**Returns:**
int - ένα πεδίο που θα εμφανίζεται στα δεξιά της μπάρας.
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


Λαμβάνει το [Shape](../../com.aspose.tasks/shape) στην αρχή της ράβδου.

**Returns:**
int - [Shape](../../com.aspose.tasks/shape) στην αρχή της μπάρας.
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


Λαμβάνει το java.awt.Color του σχήματος στην αρχή της ράβδου.

**Returns:**
java.awt.Color - ένα χρώμα του σχήματος στην αρχή της μπάρας.
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


Λαμβάνει έναν τύπο του αρχικού σχήματος.

**Returns:**
int - ένας τύπος του σχήματος εκκίνησης.
### getTextStyle() {#getTextStyle--}
```
public final TextStyle getTextStyle()
```


Λαμβάνει το στυλ του κειμένου της ράβδου.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - style of the bar's text.
### getTo() {#getTo--}
```
public final int getTo()
```


Λαμβάνει τη θέση του τελικού σημείου της μπάρας gantt.

**Returns:**
int - θέση του τελικού σημείου της μπάρας gantt.
### getTopBarTextConverter() {#getTopBarTextConverter--}
```
public final TaskBarTextConverter getTopBarTextConverter()
```


Λαμβάνει τον μετατροπέα που ορίζεται από τον χρήστη για να λαμβάνει κείμενο που θα αποτυπώνεται στην κορυφή της μπάρας της εργασίας. Αντικαθιστά την τιμή της `TopField`([getTopField()](../../com.aspose.tasks/barstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/barstyle\#setTopField-int-)) ιδιότητας.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


Λαμβάνει ένα πεδίο που θα εμφανίζεται στο πάνω μέρος της ράβδου.

**Returns:**
int - ένα πεδίο που θα εμφανίζεται στην κορυφή της μπάρας.
### setBarColor(Color value) {#setBarColor-java.awt.Color-}
```
public final void setBarColor(Color value)
```


Ορίζει το java.awt.Color του στυλ ράβδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | ένα χρώμα του στυλ της μπάρας. |

### setBarShape(int value) {#setBarShape-int-}
```
public final void setBarShape(int value)
```


Ορίζει το `BarShape`([getBarShape()](../../com.aspose.tasks/barstyle\#getBarShape--)/[setBarShape(int)](../../com.aspose.tasks/barstyle\#setBarShape-int-)) του στυλ ράβδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | [BarShape](../../com.aspose.tasks/barshape) του στυλ της μπάρας. |

### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


Ορίζει τον μετατροπέα που ορίζεται από τον χρήστη για να λαμβάνει κείμενο που θα αποτυπώνεται στο κάτω μέρος της μπάρας της εργασίας. Αντικαθιστά την τιμή της `BottomField`([getBottomField()](../../com.aspose.tasks/barstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/barstyle\#setBottomField-int-)) ιδιότητας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί στο κάτω μέρος της μπάρας της εργασίας. |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


Ορίζει ένα πεδίο που θα εμφανίζεται στο κάτω μέρος της ράβδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα πεδίο που θα εμφανίζεται στο κάτω μέρος της μπάρας. |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


Ορίζει το [Shape](../../com.aspose.tasks/shape) στο τέλος της ράβδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | [Shape](../../com.aspose/tasks/shape) στο τέλος της μπάρας. |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


Ορίζει το java.awt.Color του σχήματος στο τέλος της ράβδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | ένα χρώμα του σχήματος στην αρχή της μπάρας. |

### setEndShapeType(int value) {#setEndShapeType-int-}
```
public final void setEndShapeType(int value)
```


Ορίζει έναν τύπο του σχήματος τέλους. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας τύπος του σχήματος τέλους. |

### setFrom(int value) {#setFrom-int-}
```
public final void setFrom(int value)
```


Ορίζει τη θέση του σημείου εκκίνησης της μπάρας gantt. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια θέση σημείου εκκίνησης της μπάρας gantt. |

### setInsideBarTextConverter(TaskBarTextConverter value) {#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setInsideBarTextConverter(TaskBarTextConverter value)
```


Ορίζει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί μέσα στη μπάρα της εργασίας. Αντικαθιστά την τιμή της `InsideField`([getInsideField()](../../com.aspose/tasks/barstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose/tasks/barstyle\#setInsideField-int-)) ιδιότητας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί μέσα στη μπάρα της εργασίας. |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


Ορίζει ένα πεδίο που θα εμφανίζεται μέσα στη ράβδο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα πεδίο που θα εμφανίζεται μέσα στη μπάρα. |

### setItemType(int value) {#setItemType-int-}
```
public final void setItemType(int value)
```


Ορίζει το [BarItemType](../../com.aspose.tasks/baritemtype) του στυλ ράβδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | [BarItemType](../../com.aspose/tasks/baritemtype) του στυλ μπάρας. |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


Ορίζει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα αριστερά της μπάρας της εργασίας. Αντικαθιστά την τιμή της `LeftField`([getLeftField()](../../com.aspose/tasks/barstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose/tasks/barstyle\#setLeftField-int-)) ιδιότητας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί στα αριστερά της μπάρας της εργασίας. |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


Ορίζει ένα πεδίο που θα εμφανίζεται στα αριστερά της ράβδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα πεδίο που θα εμφανίζεται στα αριστερά της μπάρας. |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


Ορίζει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα δεξιά της μπάρας της εργασίας. Αντικαθιστά την τιμή της `RightField`([getRightField()](../../com.aspose/tasks/barstyle\#getRightField--)/[setRightField(int)](../../com.aspose/tasks/barstyle\#setRightField-int-)) ιδιότητας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας ορισμένος από τον χρήστη για λήψη κειμένου που θα αποδοθεί στα δεξιά της μπάρας της εργασίας. |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


Ορίζει ένα πεδίο που θα εμφανίζεται στα δεξιά της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα πεδίο που θα εμφανίζεται στα δεξιά της μπάρας. |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


Ορίζει το [Shape](../../com.aspose.tasks/shape) στην αρχή της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | [Shape](../../com.aspose/tasks/shape) στην αρχή της μπάρας. |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


Ορίζει το java.awt.Color του σχήματος στην αρχή της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | ένα χρώμα του σχήματος στην αρχή της μπάρας. |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


Ορίζει έναν τύπο του αρχικού σχήματος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας τύπος του αρχικού σχήματος. |

### setTextStyle(TextStyle value) {#setTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setTextStyle(TextStyle value)
```


Ορίζει το στυλ του κειμένου της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | στυλ του κειμένου της μπάρας. |

### setTo(int value) {#setTo-int-}
```
public final void setTo(int value)
```


Ορίζει τη θέση του τελικού σημείου της μπάρας gantt.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια θέση του τελικού σημείου της μπάρας Gantt. |

### setTopBarTextConverter(TaskBarTextConverter value) {#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setTopBarTextConverter(TaskBarTextConverter value)
```


Ορίζει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στην κορυφή της μπάρας της εργασίας. Αντικαθιστά την τιμή της `TopField`([getTopField()](../../com.aspose/tasks/barstyle\#getTopField--)/[setTopField(int)](../../com.aspose/tasks/barstyle\#setTopField-int-)) ιδιότητας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας ορισμένος από τον χρήστη για λήψη κειμένου που θα αποδοθεί στην κορυφή της μπάρας της εργασίας. |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


Ορίζει ένα πεδίο που θα εμφανίζεται στην κορυφή της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα πεδίο που θα εμφανίζεται στην κορυφή της μπάρας. |

