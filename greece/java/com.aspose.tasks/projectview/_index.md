---
title: "ProjectView"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Κλάση προβολής Projects."
type: docs
weight: 228
url: /el/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Κλάση προβολής του έργου
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ProjectView](../../com.aspose.tasks/projectview). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getColumns()](#getColumns--) | Λαμβάνει τις στήλες προβολής του έργου. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Περιλαμβάνει στήλες Uid, όνομα εργασίας, όνομα πόρου, εργασία και διάρκεια ανάθεσης. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Περιλαμβάνει id, δείκτες, όνομα, διάρκεια, έναρξη και λήξη στηλών εργασίας. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Περιλαμβάνει Uid, όνομα πόρου, τύπο, ετικέτα υλικού, αρχικά, ομάδα, μέγιστες μονάδες, τυπική τιμή, τιμή υπερωρίας, κόστος ανά χρήση, συσσωμάτωση σε, βασικό ημερολόγιο και στήλες κώδικα πόρου. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Περιλαμβάνει Uid, όνομα, έναρξη, λήξη και στήλες πόρων εργασίας. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Περιλαμβάνει id, δείκτες, όνομα, διάρκεια, έναρξη, λήξη, προγόνους και ονόματα πόρων στηλών εργασίας. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ProjectView](../../com.aspose.tasks/projectview).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| στήλες | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | Μια λίστα των στηλών προβολής. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Λαμβάνει τις στήλες προβολής του έργου.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - οι στήλες προβολής του έργου.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Περιλαμβάνει στήλες Uid, όνομα εργασίας, όνομα πόρου, εργασία και διάρκεια ανάθεσης.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Περιλαμβάνει id, δείκτες, όνομα, διάρκεια, έναρξη και λήξη στηλών εργασίας.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Περιλαμβάνει Uid, όνομα πόρου, τύπο, ετικέτα υλικού, αρχικά, ομάδα, μέγιστες μονάδες, τυπική τιμή, τιμή υπερωρίας, κόστος ανά χρήση, συσσωμάτωση σε, βασικό ημερολόγιο και στήλες κώδικα πόρου.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Περιλαμβάνει Uid, όνομα, έναρξη, λήξη και στήλες πόρων εργασίας.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Περιλαμβάνει id, δείκτες, όνομα, διάρκεια, έναρξη, λήξη, προγόνους και ονόματα πόρων στηλών εργασίας.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
