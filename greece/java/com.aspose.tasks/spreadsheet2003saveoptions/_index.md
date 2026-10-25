---
title: "Spreadsheet2003SaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε Spreadsheet2003."
type: docs
weight: 280
url: /el/java/com.aspose.tasks/spreadsheet2003saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class Spreadsheet2003SaveOptions extends SimpleSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε Spreadsheet2003.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Spreadsheet2003SaveOptions()](#Spreadsheet2003SaveOptions--) | Αρχικοποιεί ένα νέο αντικείμενο της [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) κλάσης. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Λαμβάνει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getResourceView()](#getResourceView--) | Λαμβάνει μια λίστα των στηλών προβολής πόρων για απόδοση ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Λαμβάνει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Ορίζει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Ορίζει μια λίστα των στηλών προβολής πόρων για απόδοση ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Ορίζει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση. |
### Spreadsheet2003SaveOptions() {#Spreadsheet2003SaveOptions--}
```
public Spreadsheet2003SaveOptions()
```


Αρχικοποιεί ένα νέο αντικείμενο της [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) κλάσης.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Λαμβάνει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
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


Λαμβάνει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Ορίζει μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | μια λίστα των στηλών προβολής εκχωρήσεων για απόδοση ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

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


Ορίζει μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | μια λίστα των στηλών προβολής ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) για αποθήκευση. |

