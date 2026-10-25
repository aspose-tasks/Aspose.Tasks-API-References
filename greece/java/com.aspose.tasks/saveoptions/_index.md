---
title: "SaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αυτή είναι μια αφηρημένη βασική κλάση για κλάσεις που επιτρέπουν στον χρήστη να καθορίζει πρόσθετες επιλογές κατά την αποθήκευση ενός έργου σε συγκεκριμένη μορφή."
type: docs
weight: 274
url: /el/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Αυτή είναι μια αφηρημένη βασική κλάση για κλάσεις που επιτρέπουν στον χρήστη να καθορίζει πρόσθετες επιλογές κατά την αποθήκευση ενός έργου σε συγκεκριμένη μορφή.

--------------------

Ένα αντικείμενο οποιασδήποτε κλάσης που προέρχεται από την κλάση SaveOptions περνάται στις υπερφορτώσεις stream Save ή string Save, ώστε ο χρήστης να ορίσει προσαρμοσμένες επιλογές κατά την αποθήκευση ενός εγγράφου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Λαμβάνει τη λίστα των αντικειμένων της κλάσης [BarStyle](../../com.aspose.tasks/barstyle) που εμφανίζονται στην προβολή του έργου. |
| [getCustomPageSize()](#getCustomPageSize--) | Λαμβάνει το προσαρμοσμένο μέγεθος σελίδας σε μονάδες point (1 point = 1/72 ίντσας). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Λαμβάνει μια τιμή που υποδεικνύει εάν ο μη εργάσιμος χρόνος πρέπει να σχεδιαστεί (Η προεπιλεγμένη τιμή είναι TRUE). |
| [getEndDate()](#getEndDate--) | Λαμβάνει μια ημερομηνία για την ολοκλήρωση της απόδοσης. |
| [getFitContent()](#getFitContent--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να ταιριάζει στο περιεχόμενό της. |
| [getGridlines()](#getGridlines--) | Λαμβάνει μια λίστα των [Gridline](../../com.aspose.tasks/gridline) που εμφανίζονται στην προβολή του έργου. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Λαμβάνει μια τιμή που ορίζει πώς θα αποδοθεί ένα υπόμνημα. |
| [getLegendItems()](#getLegendItems--) | Λαμβάνει έναν πίνακα των PageLegendItem που ορίζουν ποιες μπάρες πρέπει να αποδοθούν στο υπόμνημα της σελίδας. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανίζονται με κόκκινο χρώμα (Η προεπιλεγμένη τιμή είναι FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Λαμβάνει το χρώμα του μη εργάσιμου χρόνου. |
| [getPageCount()](#getPageCount--) | Λαμβάνει τον αριθμό των σελίδων του έργου. |
| [getPageSize()](#getPageSize--) | Λαμβάνει το μέγεθος της σελίδας που θα αποδοθεί (Η προεπιλεγμένη τιμή είναι PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Λαμβάνει το `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) στο οποίο θα αποθηκευτεί το έγγραφο. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Λαμβάνει μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι υποεργασίες στη γραμμή περίληψης εργασίας πρέπει να σημειωθούν. |
| [getStartDate()](#getStartDate--) | Λαμβάνει την ημερομηνία από την οποία θα ξεκινήσει η απόδοση. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Λαμβάνει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή ορισμένων πτυχών της απόδοσης συνδέσμων εργασιών. |
| [getTextStyles()](#getTextStyles--) | Λαμβάνει τη λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου. |
| [getTimescale()](#getTimescale--) | Λαμβάνει την τιμή `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (αν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Λαμβάνει μια συμπεριφορά που ορίζει πώς θα ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το τέλος της σελίδας. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα πρέπει να χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση του διαγράμματος Gantt. |
| [getView()](#getView--) | Λαμβάνει μια λίστα των στηλών προβολής που θα αποδοθούν ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Λαμβάνει μια προβολή (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) για απόδοση. |
| [isPortrait()](#isPortrait--) | Λαμβάνει μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι κατακόρυφος· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι οριζόντιος. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Ορίζει τη λίστα των στιγμιοτύπων της κλάσης [BarStyle](../../com.aspose.tasks/barstyle) που εμφανίζονται στην προβολή του έργου. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Ορίζει το προσαρμοσμένο μέγεθος σελίδας σε σημεία (1 σημείο = 1/72 ίντσας). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ο μη εργάσιμος χρόνος πρέπει να σχεδιαστεί (η προεπιλεγμένη τιμή είναι TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Ορίζει μια ημερομηνία για να ολοκληρωθεί η απόδοση. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να χωρά το περιεχόμενό της. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Ορίζει μια λίστα των [Gridline](../../com.aspose.tasks/gridline) που εμφανίζονται στην προβολή του έργου. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Ορίζει μια τιμή που καθορίζει πώς θα αποδοθεί ένα υπόμνημα. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Ορίζει έναν πίνακα των PageLegendItem που καθορίζουν ποιες μπάρες πρέπει να αποδοθούν στο υπόμνημα της σελίδας. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανιστούν με κόκκινο χρώμα (η προεπιλεγμένη τιμή είναι FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Ορίζει το χρώμα του μη εργάσιμου χρόνου. |
| [setPageSize(int value)](#setPageSize-int-) | Ορίζει το μέγεθος της σελίδας που θα αποδοθεί (η προεπιλεγμένη τιμή είναι PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι κατακόρυφος· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι οριζόντιος. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Ορίζει το `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) στο οποίο θα αποθηκευτεί το έγγραφο. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι υποεργασίες στη γραμμή περίληψης εργασίας πρέπει να σημειωθούν. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Ορίζει την ημερομηνία από την οποία ξεκινά η απόδοση. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Ορίζει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή ορισμένων πτυχών της απόδοσης των συνδέσμων εργασιών. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Ορίζει τη λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου. |
| [setTimescale(int value)](#setTimescale-int-) | Ορίζει την τιμή του `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (εάν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Ορίζει μια συμπεριφορά που καθορίζει πώς να ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το άκρο της σελίδας. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα πρέπει να χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση του διαγράμματος Gantt. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Ορίζει μια λίστα των στηλών προβολής που θα αποδοθούν ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Ορίζει μια προβολή (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) για απόδοση. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Λαμβάνει τη λίστα των αντικειμένων της κλάσης [BarStyle](../../com.aspose.tasks/barstyle) που εμφανίζονται στην προβολή του έργου.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - η λίστα των στιγμιοτύπων της κλάσης [BarStyle](../../com.aspose.tasks/barstyle) που εμφανίζονται στην προβολή έργου.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Λαμβάνει το προσαρμοσμένο μέγεθος σελίδας σε μονάδες point (1 point = 1/72 ίντσας).

**Returns:**
java.awt.geom.Dimension2D - το προσαρμοσμένο μέγεθος σελίδας σε μονάδες (1 μονάδα = 1/72 ίντσας).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν ο μη εργάσιμος χρόνος πρέπει να σχεδιαστεί (Η προεπιλεγμένη τιμή είναι TRUE).

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν ο μη εργάσιμος χρόνος πρέπει να σχεδιαστεί (Η προεπιλεγμένη τιμή είναι TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Λαμβάνει μια ημερομηνία για την ολοκλήρωση της απόδοσης.

**Returns:**
java.util.Date - μια ημερομηνία μέχρι την οποία θα ολοκληρωθεί η απόδοση.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να ταιριάζει στο περιεχόμενό της.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να χωρά το περιεχόμενό της.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Λαμβάνει μια λίστα των [Gridline](../../com.aspose.tasks/gridline) που εμφανίζονται στην προβολή του έργου.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - μια λίστα των [Gridline](../../com.aspose.tasks/gridline) που εμφανίζονται στην προβολή έργου.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Λαμβάνει μια τιμή που καθορίζει πώς να αποδοθεί ένα υπόμνημα. Η προεπιλεγμένη τιμή είναι LegendDrawingOptions.OnEveryPage.

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Returns:**
int - μια τιμή που καθορίζει πώς να αποδοθεί ένα υπόμνημα.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Λαμβάνει έναν πίνακα των PageLegendItem που καθορίζουν ποιοι ράβδοι πρέπει να αποδοθούν στο υπόμνημα της σελίδας. Εάν είναι null, αποδίδονται τα προεπιλεγμένα στοιχεία.

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Returns:**
com.aspose.tasks.PageLegendItem[] - ένας πίνακας των PageLegendItem που καθορίζουν ποιοι ράβδοι πρέπει να αποδοθούν στο υπόμνημα της σελίδας.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανίζονται με κόκκινο χρώμα (Η προεπιλεγμένη τιμή είναι FALSE).

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανίζονται με κόκκινο χρώμα (Η προεπιλεγμένη τιμή είναι FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Λαμβάνει το χρώμα του μη εργάσιμου χρόνου.

**Returns:**
java.awt.Color - το χρώμα του μη εργάσιμου χρόνου.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Λαμβάνει τον αριθμό των σελίδων του έργου.

**Returns:**
int - ο αριθμός των σελίδων του έργου.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Λαμβάνει το μέγεθος της σελίδας που θα αποδοθεί (Η προεπιλεγμένη τιμή είναι PageSize.A4).

**Returns:**
int - το μέγεθος της σελίδας που θα αποδοθεί (Η προεπιλεγμένη τιμή είναι PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Λαμβάνει το `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) στο οποίο θα αποθηκευτεί το έγγραφο.

**Returns:**
int - το `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) στο οποίο θα αποθηκευτεί το έγγραφο.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία μόνο σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. Το μέγεθος της σελίδας θα αλλάξει ώστε το αποδοθέν έργο να χωράει σε μία σελίδα.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία μόνο σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι υποεργασίες στη γραμμή περίληψης εργασίας πρέπει να σημειωθούν. Για τις υποεργασίες, το πεδίο Rollup υποδεικνύει εάν οι πληροφορίες στις γραμμές Gantt των υποεργασιών θα συγκεντρωθούν στη γραμμή περίληψης εργασίας. Για τις εργασίες περίληψης, το πεδίο Rollup υποδεικνύει εάν η γραμμή περίληψης εργασίας εμφανίζει συγκεντρωμένες γραμμές. Πρέπει να έχετε το πεδίο Rollup για τις εργασίες περίληψης ορισμένο σε Ναι για να συγκεντρωθούν σε αυτό οποιεσδήποτε υποεργασίες.

--------------------

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν οι υποεργασίες στη γραμμή περίληψης εργασίας πρέπει να σημειωθούν.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Λαμβάνει την ημερομηνία από την οποία θα ξεκινήσει η απόδοση.

**Returns:**
java.util.Date - η ημερομηνία από την οποία ξεκινά η απόδοση.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Λαμβάνει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή ορισμένων πτυχών της απόδοσης συνδέσμων εργασιών.

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Λαμβάνει τη λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου.

--------------------

Αυτά τα στυλ αντικαθιστούν τα στυλ που ορίζονται με το GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - η λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Λαμβάνει την τιμή `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (αν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή.

**Returns:**
int - η τιμή του `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (εάν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Λαμβάνει μια συμπεριφορά που ορίζει πώς θα ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το τέλος της σελίδας.

**Returns:**
int - μια συμπεριφορά που ορίζει πώς να ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το άκρο της σελίδας.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα πρέπει να χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση του διαγράμματος Gantt.

--------------------

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν πρέπει να χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση του διαγράμματος Gantt.
### getView() {#getView--}
```
public final ProjectView getView()
```


Λαμβάνει μια λίστα των στηλών προβολής που θα αποδοθούν ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Εάν δεν οριστεί, τότε αποδίδονται μόνο τα IDs εργασιών, τα ονόματα εργασιών, η έναρξη και η λήξη. Εάν τόσο η View όσο και οι ιδιότητες `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) είναι ορισμένες, οι στήλες από τη View αντικαθιστούν τις στήλες από το ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Λαμβάνει μια προβολή (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) για απόδοση. Μπορείτε να χρησιμοποιήσετε αυτήν την επιλογή για να καθορίσετε ρητά ποια προβολή πρέπει να αποθηκευτεί σε μορφές PDF, HTML ή Image. Εάν αυτή η ιδιότητα οριστεί, η ιδιότητα [PresentationFormat](../../com.aspose.tasks/presentationformat) αγνοείται όταν το έργο αποθηκεύεται. Η προβολή πρέπει να προέρχεται από μία από τις ακόλουθες οθόνες ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι κατακόρυφος· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι οριζόντιος.

--------------------

Δεν ισχύει όταν SaveOptions.getPageSize() == PageSize.DefinedInView. Σε αυτήν την περίπτωση χρησιμοποιείται το [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) αντί αυτού. Δεν ισχύει όταν έχει οριστεί το [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--).

**Returns:**
boolean - τιμή που υποδεικνύει αν ο προσανατολισμός της σελίδας είναι πορτραίτο· επιστρέφει false εάν ο προσανατολισμός είναι τοπίο.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Ορίζει τη λίστα των στιγμιοτύπων της κλάσης [BarStyle](../../com.aspose.tasks/barstyle) που εμφανίζονται στην προβολή του έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | η λίστα των στιγμιοτύπων της κλάσης [BarStyle](../../com.aspose.tasks/barstyle) που εμφανίζονται στην προβολή του έργου. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Ορίζει το προσαρμοσμένο μέγεθος σελίδας σε σημεία (1 σημείο = 1/72 ίντσας).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.geom.Dimension2D | το προσαρμοσμένο μέγεθος σελίδας σε σημεία (1 σημείο = 1/72 ίντσας). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν ο μη εργάσιμος χρόνος πρέπει να σχεδιαστεί (η προεπιλεγμένη τιμή είναι TRUE).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν πρέπει να σχεδιαστεί μη εργάσιμη ώρα (Η προεπιλεγμένη τιμή είναι TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Ορίζει μια ημερομηνία για να ολοκληρωθεί η απόδοση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια ημερομηνία για να ολοκληρωθεί η απόδοση. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να χωρά το περιεχόμενό της.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να χωρά το περιεχόμενό της. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Ορίζει μια λίστα των [Gridline](../../com.aspose.tasks/gridline) που εμφανίζονται στην προβολή του έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | μια λίστα των [Gridline](../../com.aspose.tasks/gridline) που εμφανίζονται στην προβολή του έργου. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Ορίζει μια τιμή που καθορίζει πώς θα αποδοθεί ένα υπόμνημα. Η προεπιλεγμένη τιμή είναι LegendDrawingOptions.OnEveryPage.

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια τιμή που καθορίζει πώς θα αποδοθεί ένα υπόμνημα. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Ορίζει έναν πίνακα των PageLegendItem που καθορίζουν ποιες γραμμές πρέπει να αποδοθούν στο υπόμνημα της σελίδας. Εάν είναι null, αποδίδονται τα προεπιλεγμένα στοιχεία.

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | ένας πίνακας των PageLegendItem που καθορίζουν ποιες γραμμές πρέπει να αποδοθούν στο υπόμνημα της σελίδας. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανιστούν με κόκκινο χρώμα (η προεπιλεγμένη τιμή είναι FALSE).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν οι κρίσιμες εργασίες πρέπει να εμφανίζονται με κόκκινο χρώμα (Η προεπιλεγμένη τιμή είναι FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Ορίζει το χρώμα του μη εργάσιμου χρόνου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | το χρώμα του μη-εργασιακού χρόνου. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Ορίζει το μέγεθος της σελίδας που θα αποδοθεί (η προεπιλεγμένη τιμή είναι PageSize.A4).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το μέγεθος της σελίδας που θα αποδοθεί (Η προεπιλεγμένη τιμή είναι PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν ο προσανατολισμός της σελίδας είναι κατακόρυφος· επιστρέφει false εάν ο προσανατολισμός της σελίδας είναι οριζόντιος.

--------------------

Δεν ισχύει όταν SaveOptions.PageSize == Visualization.PageSize.DefinedInView. Σε αυτήν την περίπτωση το [PageSettings.setPortrait(boolean)](../../com.aspose/tasks/pagesettings\#setPortrait-boolean-) χρησιμοποιείται αντ' αυτού. Δεν ισχύει όταν το [getCustomPageSize()](../../com.aspose/tasks/saveoptions\#getCustomPageSize--) είναι ορισμένο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει αν ο προσανατολισμός της σελίδας είναι πορτραίτο· επιστρέφει false εάν ο προσανατολισμός είναι τοπίο. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Ορίζει το `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) στο οποίο θα αποθηκευτεί το έγγραφο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | το `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) στο οποίο θα αποθηκευτεί το έγγραφο. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία μόνο σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. Το μέγεθος της σελίδας θα αλλάξει ώστε το αποδοθέν έργο να χωράει σε μία σελίδα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν ένα έργο πρέπει να αποδοθεί σε μία μόνο σελίδα όταν το έργο αποθηκεύεται σε γραφική μορφή. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν τα υπο-έργα στη γραμμή σύνοψης εργασίας πρέπει να σημειωθούν. Για τα υπο-έργα, το πεδίο Rollup υποδεικνύει εάν οι πληροφορίες στις γραμμές Gantt των υπο-έργων θα συγκεντρωθούν στη γραμμή σύνοψης εργασίας. Για τις εργασίες σύνοψης, το πεδίο Rollup υποδεικνύει εάν η γραμμή σύνοψης εργασίας εμφανίζει συγκεντρωμένες γραμμές. Πρέπει να έχετε το πεδίο Rollup για τις εργασίες σύνοψης ορισμένο σε Yes ώστε οποιαδήποτε υπο-έργα να συγκεντρωθούν σε αυτές.

--------------------

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν τα υπο-έργα στη γραμμή σύνοψης εργασίας πρέπει να σημειωθούν. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Ορίζει την ημερομηνία από την οποία ξεκινά η απόδοση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η ημερομηνία από την οποία θα ξεκινήσει η απόδοση. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Ορίζει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή ορισμένων πτυχών της απόδοσης των συνδέσμων εργασιών.

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή ορισμένων πτυχών της απόδοσης συνδέσμων εργασιών. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Ορίζει τη λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου.

--------------------

Αυτά τα στυλ αντικαθιστούν τα στυλ που ορίζονται με το GanttCharView.setTextStyles.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | η λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Ορίζει την τιμή του `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (εάν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | η τιμή του `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) που χρησιμοποιείται για τον έλεγχο του τρόπου απόδοσης της κλίμακας χρόνου (εάν υπάρχει) όταν το έργο αποθηκεύεται σε γραφική μορφή. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Ορίζει μια συμπεριφορά που καθορίζει πώς να ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το άκρο της σελίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια συμπεριφορά που ορίζει πώς να ευθυγραμμιστεί το δεξιό άκρο της κλίμακας χρόνου με το άκρο της σελίδας. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα πρέπει να χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση του διαγράμματος Gantt.

--------------------

Ισχύει μόνο όταν αποδίδεται η προβολή διαγράμματος Gantt.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν θα πρέπει να χρησιμοποιηθεί διαβάθμιση πινέλου κατά την απόδοση του διαγράμματος Gantt. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Ορίζει μια λίστα των στηλών προβολής που θα αποδοθούν ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Εάν δεν οριστεί, τότε αποδίδονται μόνο τα IDs εργασιών, τα ονόματα εργασιών, η έναρξη και η λήξη. Εάν τόσο το View όσο και τις ιδιότητες `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) έχουν οριστεί, οι στήλες από το View υπερισχύουν των στηλών από το ViewSettings.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | μια λίστα των στηλών προβολής που θα αποδοθούν ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Ορίζει μια προβολή (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) για απόδοση. Μπορείτε να χρησιμοποιήσετε αυτήν την επιλογή για να καθορίσετε ρητά ποια προβολή θα αποθηκευτεί σε μορφές PDF, HTML ή Image. Εάν αυτή η ιδιότητα οριστεί, η ιδιότητα [PresentationFormat](../../com.aspose.tasks/presentationformat) αγνοείται όταν το έργο αποθηκεύεται. Η προβολή πρέπει να προέρχεται από μία από τις ακόλουθες οθόνες ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | μια προβολή (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) για απόδοση. |

