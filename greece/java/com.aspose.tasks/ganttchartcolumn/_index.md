---
title: "GanttChartColumn"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Κλάση προβολής Projects."
type: docs
weight: 111
url: /el/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Κλάση προβολής του έργου
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Μετατρέπει την τρέχουσα εργασία σε κείμενο στήλης. |
| [getField()](#getField--) | Επιστρέφει το πεδίο της στήλης. |
| [setField(int value)](#setField-int-) | Ορίζει το πεδίο της στήλης. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Όνομα στήλης. |
| width | int | Πλάτος στήλης σε εικονοστοιχεία. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Μετατροπέας δεδομένων εργασίας σε κείμενο στήλης. |
| πεδίο | int | Πεδίο στήλης. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Όνομα στήλης. |
| width | int | Πλάτος στήλης σε εικονοστοιχεία. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Μετατροπέας δεδομένων εργασίας σε κείμενο στήλης. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| width | int | Πλάτος στήλης σε εικονοστοιχεία. |
| πεδίο | int | Πεδίο στήλης. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης GanttChartColumn.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | java.lang.String | Όνομα στήλης. |
| width | int | Πλάτος στήλης σε εικονοστοιχεία. |
| πεδίο | int | Πεδίο στήλης. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Μετατρέπει την τρέχουσα εργασία σε κείμενο στήλης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Τρέχουσα εργασία. |

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

