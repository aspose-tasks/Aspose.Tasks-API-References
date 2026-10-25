---
title: "XlsxOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά τη μετατροπή σελίδων έργου σε XLSX."
type: docs
weight: 368
url: /el/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά τη μετατροπή σελίδων έργου σε XLSX.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XlsxOptions](../../com.aspose.tasks/xlsxoptions) που μπορεί να χρησιμοποιηθεί για αποθήκευση του έργου σε μορφή XLSX. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Λαμβάνει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Λαμβάνει την κωδικοποίηση του τελικού αρχείου XLSX. |
| [getResourceView()](#getResourceView--) | Λαμβάνει μια λίστα των στηλών προβολής πόρων για απόδοση ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Λαμβάνει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Ορίζει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ορίζει την κωδικοποίηση του τελικού αρχείου XLSX. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Ορίζει μια λίστα των στηλών προβολής πόρων για απόδοση ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Ορίζει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XlsxOptions](../../com.aspose.tasks/xlsxoptions) που μπορεί να χρησιμοποιηθεί για αποθήκευση του έργου σε μορφή XLSX.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Λαμβάνει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Λαμβάνει την κωδικοποίηση του τελικού αρχείου XLSX. Η προεπιλεγμένη τιμή είναι java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - η κωδικοποίηση του τελικού αρχείου XLSX.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Λαμβάνει μια λίστα των στηλών προβολής πόρων για απόδοση ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


Λαμβάνει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Ορίζει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ορίζει την κωδικοποίηση του τελικού αρχείου XLSX. Η προεπιλεγμένη τιμή είναι java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.nio.charset.Charset | η κωδικοποίηση του τελικού αρχείου XLSX. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Ορίζει μια λίστα των στηλών προβολής πόρων για απόδοση ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | μια λίστα των στηλών προβολής πόρων για απόδοση ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Ορίζει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση σε μορφή XLSX. |

