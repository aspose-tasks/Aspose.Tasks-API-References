---
title: "GanttBarStyle"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά ένα στυλ ράβδου που χρησιμοποιείται από το MSP στην προβολή Διαγράμματος Gantt."
type: docs
weight: 109
url: /el/java/com.aspose.tasks/ganttbarstyle/
---

**Inheritance:**
java.lang.Object
```
public class GanttBarStyle
```

Αναπαριστά ένα στυλ ράβδου που χρησιμοποιείται από το MSP στην προβολή Διαγράμματος Gantt.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GanttBarStyle()](#GanttBarStyle--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στο κάτω μέρος της γραμμής της εργασίας. |
| [getBottomField()](#getBottomField--) | Λαμβάνει τα δεδομένα που θα εμφανιστούν στο κάτω μέρος της γραμμής. |
| [getEndShape()](#getEndShape--) | Λαμβάνει το σχήμα τέλους της γραμμής. |
| [getEndShapeColor()](#getEndShapeColor--) | Λαμβάνει το χρώμα του σχήματος τέλους. |
| [getEndShapeType()](#getEndShapeType--) | Λαμβάνει τον τύπο του σχήματος τέλους. |
| [getFrom()](#getFrom--) | Λαμβάνει τη θέση του σημείου εκκίνησης της γραμμής gantt. |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί μέσα στη γραμμή της εργασίας. |
| [getInsideField()](#getInsideField--) | Λαμβάνει τα δεδομένα που θα εμφανιστούν μέσα στη γραμμή. |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα αριστερά της γραμμής της εργασίας. |
| [getLeftField()](#getLeftField--) | Λαμβάνει τα δεδομένα που θα εμφανιστούν στα αριστερά της γραμμής. |
| [getMiddleFillPattern()](#getMiddleFillPattern--) | Λαμβάνει το μοτίβο γεμίσματος της γραμμής gantt. |
| [getMiddleShape()](#getMiddleShape--) | Λαμβάνει το μεσαίο σχήμα της γραμμής. |
| [getMiddleShapeColor()](#getMiddleShapeColor--) | Λαμβάνει ένα χρώμα του μεσαίου σχήματος. |
| [getName()](#getName--) | Λαμβάνει ένα όνομα του στυλ. |
| [getParentStyle()](#getParentStyle--) | Λαμβάνει το γονικό (ή κοινό) στυλ για προσαρμοσμένο στυλ συγκεκριμένου έργου. |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα δεξιά της μπάρας του έργου. |
| [getRightField()](#getRightField--) | Λαμβάνει τα δεδομένα που θα εμφανιστούν στα δεξιά της μπάρας. |
| [getRow()](#getRow--) | Λαμβάνει έναν αριθμό γραμμής. |
| [getShowForCategories()](#getShowForCategories--) | Λαμβάνει τις κατηγορίες εργασιών για τις οποίες εφαρμόζεται το στυλ. |
| [getShowForTaskUid()](#getShowForTaskUid--) | Λαμβάνει το μοναδικό Id μιας εργασίας για την οποία εφαρμόζεται το στυλ. |
| [getStartShape()](#getStartShape--) | Λαμβάνει το αρχικό σχήμα της μπάρας. |
| [getStartShapeColor()](#getStartShapeColor--) | Λαμβάνει ένα χρώμα του αρχικού σχήματος. |
| [getStartShapeType()](#getStartShapeType--) | Λαμβάνει έναν τύπο του αρχικού σχήματος. |
| [getTo()](#getTo--) | Λαμβάνει τη θέση του τελικού σημείου της μπάρας gantt. |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | Λαμβάνει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στην κορυφή της μπάρας του έργου. |
| [getTopField()](#getTopField--) | Λαμβάνει τα δεδομένα που θα εμφανιστούν στην κορυφή της μπάρας. |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στο κάτω μέρος της μπάρας του έργου. |
| [setBottomField(int value)](#setBottomField-int-) | Ορίζει τα δεδομένα που θα εμφανιστούν στο κάτω μέρος της μπάρας. |
| [setEndShape(int value)](#setEndShape-int-) | Ορίζει ένα τελικό σχήμα της μπάρας. |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | Ορίζει ένα χρώμα του τελικού σχήματος. |
| [setEndShapeType(int value)](#setEndShapeType-int-) | Ορίζει έναν τύπο του τελικού σχήματος. |
| [setFrom(int value)](#setFrom-int-) | Ορίζει τη θέση του αρχικού σημείου της μπάρας gantt. |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί μέσα στη μπάρα του έργου. |
| [setInsideField(int value)](#setInsideField-int-) | Ορίζει τα δεδομένα που θα εμφανιστούν μέσα στη μπάρα. |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει τον μετατροπέα που ορίζεται από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα αριστερά της μπάρας του έργου. |
| [setLeftField(int value)](#setLeftField-int-) | Ορίζει τα δεδομένα που θα εμφανιστούν στα αριστερά της μπάρας. |
| [setMiddleFillPattern(int value)](#setMiddleFillPattern-int-) | Ορίζει ένα μοτίβο γεμίσματος της μπάρας gantt. |
| [setMiddleShape(int value)](#setMiddleShape-int-) | Ορίζει ένα μεσαίο σχήμα της μπάρας. |
| [setMiddleShapeColor(Color value)](#setMiddleShapeColor-java.awt.Color-) | Ορίζει ένα χρώμα του μεσαίου σχήματος. |
| [setName(String value)](#setName-java.lang.String-) | Ορίζει ένα όνομα του στυλ. |
| [setParentStyle(GanttBarStyle value)](#setParentStyle-com.aspose.tasks.GanttBarStyle-) | Ορίζει το γονικό (ή κοινό) στυλ για προσαρμοσμένο στυλ συγκεκριμένου έργου. |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στα δεξιά της μπάρας του έργου. |
| [setRightField(int value)](#setRightField-int-) | Ορίζει τα δεδομένα που θα εμφανιστούν στα δεξιά της μπάρας. |
| [setRow(int value)](#setRow-int-) | Ορίζει έναν αριθμό γραμμής. |
| [setShowForCategories(List&lt;Integer&gt; value)](#setShowForCategories-java.util.List-java.lang.Integer--) | Ορίζει τις κατηγορίες εργασιών για τις οποίες εφαρμόζεται το στυλ. |
| [setShowForTaskUid(Integer value)](#setShowForTaskUid-java.lang.Integer-) | Ορίζει το μοναδικό αναγνωριστικό Unique Id μιας εργασίας για την οποία εφαρμόζεται το στυλ. |
| [setStartShape(int value)](#setStartShape-int-) | Ορίζει ένα αρχικό σχήμα της μπάρας. |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | Ορίζει ένα χρώμα του αρχικού σχήματος. |
| [setStartShapeType(int value)](#setStartShapeType-int-) | Ορίζει έναν τύπο του αρχικού σχήματος. |
| [setTo(int value)](#setTo-int-) | Ορίζει τη θέση του τελικού σημείου της μπάρας gantt. |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ορίζει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στην κορυφή της μπάρας του έργου. |
| [setTopField(int value)](#setTopField-int-) | Ορίζει τα δεδομένα που θα εμφανιστούν στην κορυφή της μπάρας. |
### GanttBarStyle() {#GanttBarStyle--}
```
public GanttBarStyle()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


Λαμβάνει μετατροπέα ορισμένο από το χρήστη για λήψη κειμένου που θα αποτυπωθεί στο κάτω μέρος της μπάρας του έργου. Αντικαθιστά την τιμή της ιδιότητας `BottomField`([getBottomField()](../../com.aspose/tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


Λαμβάνει τα δεδομένα που θα εμφανιστούν στο κάτω μέρος της μπάρας. [Field](../../com.aspose.tasks/field).

**Returns:**
int - δεδομένα που θα εμφανιστούν στο κάτω μέρος της μπάρας.
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


Λαμβάνει το σχήμα τέλους της γραμμής.

**Returns:**
int - ένα τελικό σχήμα της μπάρας.
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


Λαμβάνει το χρώμα του σχήματος τέλους.

**Returns:**
java.awt.Color - ένα χρώμα του τελικού σχήματος.
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


Λαμβάνει τον ορισμένο από τον χρήστη μετατροπέα για να πάρει το κείμενο που θα αποδοθεί μέσα στη μπάρα της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `InsideField`([getInsideField()](../../com.aspose/tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose/tasks/ganttbarstyle\#setInsideField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


Λαμβάνει τα δεδομένα που θα εμφανιστούν μέσα στη μπάρα. [Field](../../com.aspose/tasks/field).

**Returns:**
int - δεδομένα που θα εμφανιστούν μέσα στη μπάρα.
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


Λαμβάνει τον ορισμένο από τον χρήστη μετατροπέα για να πάρει το κείμενο που θα αποδοθεί στα αριστερά της μπάρας της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `LeftField`([getLeftField()](../../com.aspose/tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose/tasks/ganttbarstyle\#setLeftField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


Λαμβάνει τα δεδομένα που θα εμφανιστούν στα αριστερά της μπάρας. [Field](../../com.aspose/tasks/field).

**Returns:**
int - δεδομένα που θα εμφανιστούν στα αριστερά της μπάρας.
### getMiddleFillPattern() {#getMiddleFillPattern--}
```
public final int getMiddleFillPattern()
```


Λαμβάνει το μοτίβο γεμίσματος της γραμμής gantt.

**Returns:**
int - ένα μοτίβο γεμίσματος της μπάρας gantt.
### getMiddleShape() {#getMiddleShape--}
```
public final int getMiddleShape()
```


Λαμβάνει το μεσαίο σχήμα της γραμμής.

**Returns:**
int - ένα μεσαίο σχήμα της μπάρας.
### getMiddleShapeColor() {#getMiddleShapeColor--}
```
public final Color getMiddleShapeColor()
```


Λαμβάνει ένα χρώμα του μεσαίου σχήματος.

**Returns:**
java.awt.Color - ένα χρώμα του μεσαίου σχήματος.
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει ένα όνομα του στυλ.

**Returns:**
java.lang.String - ένα όνομα του στυλ.
### getParentStyle() {#getParentStyle--}
```
public final GanttBarStyle getParentStyle()
```


Λαμβάνει το γονικό (ή κοινό) στυλ για προσαρμοσμένο στυλ συγκεκριμένου έργου.

--------------------

Μια εργασία μπορεί να έχει πολλαπλά προσαρμοσμένα στυλ με διαφορετικά γονικά στυλ. Για παράδειγμα, σκεφτείτε μια εργασία που έχει προσαρμοσμένο στυλ με γονικό στυλ "Critical" και ένα άλλο στυλ με γονικό στυλ "Normal". Συνοπτικά, εάν η εργασία είναι κρίσιμη, εφαρμόζεται το πρώτο στυλ. Εάν η εργασία γίνει μη κρίσιμη, εφαρμόζεται το δεύτερο στυλ (αυτή η λογική κληρονομείται από το Microsoft Project Professional).

**Returns:**
[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) - parent (or common) style for custom task-specific style.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


Λαμβάνει τον ορισμένο από τον χρήστη μετατροπέα για να πάρει το κείμενο που θα αποδοθεί στα δεξιά της μπάρας της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `RightField`([getRightField()](../../com.aspose/tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose/tasks/ganttbarstyle\#setRightField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


Λαμβάνει τα δεδομένα που θα εμφανιστούν στα δεξιά της μπάρας. [Field](../../com.aspose/tasks/field).

**Returns:**
int - δεδομένα που θα εμφανιστούν στα δεξιά της μπάρας.
### getRow() {#getRow--}
```
public final int getRow()
```


Λαμβάνει έναν αριθμό γραμμής.

--------------------

Μπορεί να είναι από 1 έως 4 (το 1 είναι η προεπιλεγμένη τιμή).

**Returns:**
int - ένας αριθμός σειράς.
### getShowForCategories() {#getShowForCategories--}
```
public final List<Integer> getShowForCategories()
```


Λαμβάνει τις κατηγορίες εργασιών για τις οποίες εφαρμόζεται το στυλ. Ισχύει για γονικά (ή κοινά) στυλ των μπαρών σε διάγραμμα Gantt (δείτε `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose/tasks/ganttchartview\#getBarStyles--))).

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - κατηγορίες εργασιών για τις οποίες εφαρμόζεται το στυλ.
### getShowForTaskUid() {#getShowForTaskUid--}
```
public final Integer getShowForTaskUid()
```


Λαμβάνει το μοναδικό Id μιας εργασίας για την οποία εφαρμόζεται το στυλ. Ισχύει για στυλ μπαρών ειδικά για εργασίες σε διάγραμμα Gantt (δείτε `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose/tasks/ganttchartview\#getCustomBarStyles--))).

**Returns:**
java.lang.Integer - Μοναδικό Id μιας εργασίας για την οποία εφαρμόζεται το στυλ.
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


Λαμβάνει το αρχικό σχήμα της μπάρας.

**Returns:**
int - ένα σχήμα εκκίνησης της μπάρας.
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


Λαμβάνει ένα χρώμα του αρχικού σχήματος.

**Returns:**
java.awt.Color - ένα χρώμα του σχήματος εκκίνησης.
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


Λαμβάνει έναν τύπο του αρχικού σχήματος.

**Returns:**
int - ένας τύπος του σχήματος εκκίνησης.
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


Λαμβάνει τον ορισμένο από τον χρήστη μετατροπέα για να πάρει το κείμενο που θα αποδοθεί στην κορυφή της μπάρας της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `TopField`([getTopField()](../../com.aspose/tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose/tasks/ganttbarstyle\#setTopField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


Λαμβάνει τα δεδομένα που θα εμφανιστούν στην κορυφή της μπάρας.

**Returns:**
int - δεδομένα που θα εμφανιστούν στην κορυφή της μπάρας.
### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


Ορίζει μετατροπέα που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί στο κάτω μέρος της μπάρας της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί στο κάτω μέρος της μπάρας της εργασίας. |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


Ορίζει δεδομένα που θα εμφανιστούν στο κάτω μέρος της μπάρας. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | δεδομένα που θα εμφανιστούν στο κάτω μέρος της μπάρας. |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


Ορίζει ένα τελικό σχήμα της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα σχήμα τέλους της μπάρας. |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


Ορίζει ένα χρώμα του τελικού σχήματος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | ένα χρώμα του σχήματος τέλους. |

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


Ορίζει μετατροπέα που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί μέσα στη μπάρα της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί μέσα στη μπάρα της εργασίας. |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


Ορίζει δεδομένα που θα εμφανιστούν μέσα στη μπάρα. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | δεδομένα που θα εμφανιστούν μέσα στη μπάρα. |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


Ορίζει μετατροπέα που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί στα αριστερά της μπάρας της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί στα αριστερά της μπάρας της εργασίας. |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


Ορίζει δεδομένα που θα εμφανιστούν στα αριστερά της μπάρας. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | δεδομένα που θα εμφανιστούν στα αριστερά της μπάρας. |

### setMiddleFillPattern(int value) {#setMiddleFillPattern-int-}
```
public final void setMiddleFillPattern(int value)
```


Ορίζει ένα μοτίβο γεμίσματος της μπάρας gantt.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα μοτίβο γεμίσματος της μπάρας gantt. |

### setMiddleShape(int value) {#setMiddleShape-int-}
```
public final void setMiddleShape(int value)
```


Ορίζει ένα μεσαίο σχήμα της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα μεσαίο σχήμα της μπάρας. |

### setMiddleShapeColor(Color value) {#setMiddleShapeColor-java.awt.Color-}
```
public final void setMiddleShapeColor(Color value)
```


Ορίζει ένα χρώμα του μεσαίου σχήματος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | ένα χρώμα του μεσαίου σχήματος. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ορίζει ένα όνομα του στυλ.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | ένα όνομα του στυλ. |

### setParentStyle(GanttBarStyle value) {#setParentStyle-com.aspose.tasks.GanttBarStyle-}
```
public final void setParentStyle(GanttBarStyle value)
```


Ορίζει το γονικό (ή κοινό) στυλ για προσαρμοσμένο στυλ συγκεκριμένου έργου.

--------------------

Μια εργασία μπορεί να έχει πολλαπλά προσαρμοσμένα στυλ με διαφορετικά γονικά στυλ. Για παράδειγμα, σκεφτείτε μια εργασία που έχει προσαρμοσμένο στυλ με γονικό στυλ "Critical" και ένα άλλο στυλ με γονικό στυλ "Normal". Συνοπτικά, εάν η εργασία είναι κρίσιμη, εφαρμόζεται το πρώτο στυλ. Εάν η εργασία γίνει μη κρίσιμη, εφαρμόζεται το δεύτερο στυλ (αυτή η λογική κληρονομείται από το Microsoft Project Professional).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) | γονικό (ή κοινό) στυλ για προσαρμοσμένο στυλ ειδικό για εργασία. |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


Ορίζει μετατροπέα που ορίζεται από τον χρήστη για την απόκτηση κειμένου που θα αποδοθεί στα δεξιά της μπάρας της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) ιδιότητα.

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας ορισμένος από τον χρήστη για λήψη κειμένου που θα αποδοθεί στα δεξιά της μπάρας της εργασίας. |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


Ορίζει τα δεδομένα που θα εμφανιστούν στα δεξιά της μπάρας. [Field](../../com.aspose/tasks/field).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Δεδομένα που θα εμφανιστούν στα δεξιά της μπάρας. |

### setRow(int value) {#setRow-int-}
```
public final void setRow(int value)
```


Ορίζει έναν αριθμό γραμμής.

--------------------

Μπορεί να είναι από 1 έως 4 (το 1 είναι η προεπιλεγμένη τιμή).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | αριθμός γραμμής. |

### setShowForCategories(List&lt;Integer&gt; value) {#setShowForCategories-java.util.List-java.lang.Integer--}
```
public final void setShowForCategories(List<Integer> value)
```


Ορίζει τις κατηγορίες εργασιών για τις οποίες εφαρμόζεται το στυλ. Ισχύει για γονικές (ή κοινές) μορφές μπαρών σε διάγραμμα Gantt (δείτε `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.List&lt;java.lang.Integer&gt; | Κατηγορίες εργασιών για τις οποίες εφαρμόζεται το στυλ. |

### setShowForTaskUid(Integer value) {#setShowForTaskUid-java.lang.Integer-}
```
public final void setShowForTaskUid(Integer value)
```


Ορίζει το μοναδικό Id μιας εργασίας για την οποία εφαρμόζεται το στυλ. Ισχύει για στυλ μπαρών ειδικών για εργασίες σε διάγραμμα Gantt (δείτε `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Integer | Μοναδικό Id μιας εργασίας για την οποία εφαρμόζεται το στυλ. |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


Ορίζει ένα αρχικό σχήμα της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα αρχικό σχήμα της μπάρας. |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


Ορίζει ένα χρώμα του αρχικού σχήματος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | ένα χρώμα του αρχικού σχήματος. |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


Ορίζει έναν τύπο του αρχικού σχήματος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας τύπος του αρχικού σχήματος. |

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


Ορίζει μετατροπέα ορισμένο από τον χρήστη για λήψη κειμένου που θα αποδοθεί στην κορυφή της μπάρας της εργασίας. Αντικαθιστά την τιμή της ιδιότητας `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)).

--------------------

Δεν αποθηκεύεται σε μορφή MPP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | Μετατροπέας ορισμένος από τον χρήστη για λήψη κειμένου που θα αποδοθεί στην κορυφή της μπάρας της εργασίας. |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


Ορίζει τα δεδομένα που θα εμφανιστούν στην κορυφή της μπάρας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Δεδομένα που θα εμφανιστούν στην κορυφή της μπάρας. |

