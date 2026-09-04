---
title: "ProgressLines"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά γραμμές προόδου σε προβολή Gantt Chart."
type: docs
weight: 219
url: /el/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

Αναπαριστά γραμμές προόδου σε προβολή Gantt Chart.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | Λαμβάνει την ημερομηνία από την οποία θα εμφανιστούν οι γραμμές προόδου. |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου από την αρχή της ημερομηνίας έναρξης του έργου. |
| [getDateFormat()](#getDateFormat--) | Λαμβάνει τη μορφή ημερομηνίας ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζεται γραμμή προόδου στην τρέχουσα ημερομηνία. |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζεται γραμμή προόδου σε επαναλαμβανόμενα διαστήματα. |
| [getDisplaySelected()](#getDisplaySelected--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου στις επιλεγμένες ημερομηνίες. |
| [getFont()](#getFont--) | Λαμβάνει τη γραμματοσειρά που χρησιμοποιείται για την ετικέτα της γραμμής προόδου. |
| [getLineColor()](#getLineColor--) | Λαμβάνει το χρώμα της γραμμής για την τρέχουσα γραμμή προόδου. |
| [getLinePattern()](#getLinePattern--) | Λαμβάνει το μοτίβο γραμμής της τρέχουσας γραμμής προόδου. |
| [getOtherLineColor()](#getOtherLineColor--) | Λαμβάνει το χρώμα της άλλης γραμμής προόδου. |
| [getOtherLinePattern()](#getOtherLinePattern--) | Λαμβάνει το μοτίβο γραμμής για την άλλη γραμμή προόδου. |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | Λαμβάνει το χρώμα του άλλου σημείου προόδου. |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | Λαμβάνει το σχήμα του σημείου προόδου της άλλης γραμμής προόδου. |
| [getProgressPointColor()](#getProgressPointColor--) | Λαμβάνει το χρώμα του σημείου προόδου. |
| [getProgressPointShape()](#getProgressPointShape--) | Λαμβάνει το σχήμα του σημείου προόδου. |
| [getRecurringInterval()](#getRecurringInterval--) | Λαμβάνει το επαναλαμβανόμενο διάστημα. |
| [getSelectedDates()](#getSelectedDates--) | Λαμβάνει τη λίστα των επιλεγμένων ημερομηνιών για τις οποίες θα εμφανίζονται γραμμές προόδου. |
| [getShowDate()](#getShowDate--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η ημερομηνία για κάθε γραμμή προόδου. |
| [isBaselinePlan()](#isBaselinePlan--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου για το βασικό σχέδιο ή το πραγματικό. |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου για το βασικό σχέδιο ή το πραγματικό. |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | Ορίζει την ημερομηνία από την οποία θα εμφανίζονται γραμμές προόδου. |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου από την αρχή της ημερομηνίας έναρξης του έργου. |
| [setDateFormat(int value)](#setDateFormat-int-) | Ορίζει τη μορφή ημερομηνίας ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται γραμμή προόδου στην τρέχουσα ημερομηνία. |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται γραμμή προόδου σε επαναλαμβανόμενα διαστήματα. |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου στις επιλεγμένες ημερομηνίες. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Ορίζει τη γραμματοσειρά που χρησιμοποιείται για την ετικέτα της γραμμής προόδου. |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | Ορίζει το χρώμα της γραμμής για την τρέχουσα γραμμή προόδου. |
| [setLinePattern(int value)](#setLinePattern-int-) | Ορίζει το μοτίβο γραμμής της τρέχουσας γραμμής προόδου. |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | Ορίζει το χρώμα της άλλης γραμμής προόδου. |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | Ορίζει το μοτίβο γραμμής για την άλλη γραμμή προόδου. |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | Ορίζει το χρώμα του άλλου σημείου προόδου. |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | Ορίζει το σχήμα του σημείου προόδου της άλλης γραμμής προόδου. |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | Ορίζει το χρώμα του σημείου προόδου. |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | Ορίζει το σχήμα του σημείου προόδου. |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | Ορίζει το επαναλαμβανόμενο διάστημα. |
| [setShowDate(boolean value)](#setShowDate-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν θα εμφανίζεται η ημερομηνία για κάθε γραμμή προόδου. |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


Λαμβάνει την ημερομηνία από την οποία θα εμφανιστούν οι γραμμές προόδου.

**Returns:**
java.util.Date - η ημερομηνία από την οποία θα εμφανίζονται οι γραμμές προόδου.
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου από την αρχή της ημερομηνίας έναρξης του έργου.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν θα εμφανίζονται οι γραμμές προόδου από την αρχή της ημερομηνίας έναρξης του έργου.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Λαμβάνει τη μορφή ημερομηνίας ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - η μορφή ημερομηνίας ([DateLabel](../../com.aspose.tasks/datelabel)).
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζεται γραμμή προόδου στην τρέχουσα ημερομηνία.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν θα εμφανίζεται η γραμμή προόδου στην τρέχουσα ημερομηνία.
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζεται γραμμή προόδου σε επαναλαμβανόμενα διαστήματα.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν θα εμφανίζεται η γραμμή προόδου σε επαναλαμβανόμενα διαστήματα.
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου στις επιλεγμένες ημερομηνίες.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν θα εμφανίζονται οι γραμμές προόδου στις επιλεγμένες ημερομηνίες.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Λαμβάνει τη γραμματοσειρά που χρησιμοποιείται για την ετικέτα της γραμμής προόδου.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


Λαμβάνει το χρώμα της γραμμής για την τρέχουσα γραμμή προόδου.

**Returns:**
java.awt.Color - το χρώμα της γραμμής για την τρέχουσα γραμμή προόδου.
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


Λαμβάνει το μοτίβο γραμμής της τρέχουσας γραμμής προόδου. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - το μοτίβο γραμμής της τρέχουσας γραμμής προόδου.
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


Λαμβάνει το χρώμα της άλλης γραμμής προόδου.

**Returns:**
java.awt.Color - το χρώμα της άλλης γραμμής προόδου.
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


Λαμβάνει το μοτίβο γραμμής για την άλλη γραμμή προόδου.

**Returns:**
int - το μοτίβο γραμμής για την άλλη γραμμή προόδου.
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


Λαμβάνει το χρώμα του άλλου σημείου προόδου.

**Returns:**
java.awt.Color - το χρώμα του άλλου σημείου προόδου.
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


Λαμβάνει το σχήμα του σημείου προόδου της άλλης γραμμής προόδου.

**Returns:**
int - το σχήμα του σημείου προόδου της άλλης γραμμής προόδου.
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


Λαμβάνει το χρώμα του σημείου προόδου.

**Returns:**
java.awt.Color - το χρώμα του σημείου προόδου.
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


Λαμβάνει το σχήμα σημείου προόδου. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - το σχήμα σημείου προόδου.
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


Λαμβάνει το επαναλαμβανόμενο διάστημα. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


Λαμβάνει τη λίστα των επιλεγμένων ημερομηνιών για τις οποίες θα εμφανίζονται γραμμές προόδου.

**Returns:**
java.util.List&lt;java.util.Date&gt; - η λίστα των επιλεγμένων ημερομηνιών για τις οποίες θα εμφανιστούν γραμμές προόδου.
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η ημερομηνία για κάθε γραμμή προόδου.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν θα εμφανίζεται η ημερομηνία για κάθε γραμμή προόδου.
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου για το βασικό σχέδιο ή το πραγματικό.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν θα εμφανίζονται γραμμές προόδου για το βασικό σχέδιο ή το πραγματικό.
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου για το βασικό σχέδιο ή το πραγματικό.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν θα εμφανίζονται γραμμές προόδου για το βασικό σχέδιο ή το πραγματικό. |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


Ορίζει την ημερομηνία από την οποία θα εμφανίζονται γραμμές προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η ημερομηνία από την οποία θα εμφανίζονται οι γραμμές προόδου. |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου από την αρχή της ημερομηνίας έναρξης του έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν θα εμφανίζονται γραμμές προόδου από την αρχή της ημερομηνίας έναρξης του έργου. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Ορίζει τη μορφή ημερομηνίας ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | η μορφή ημερομηνίας ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται γραμμή προόδου στην τρέχουσα ημερομηνία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν θα εμφανίζεται η γραμμή προόδου στην τρέχουσα ημερομηνία. |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται γραμμή προόδου σε επαναλαμβανόμενα διαστήματα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν θα εμφανίζεται η γραμμή προόδου σε επαναλαμβανόμενα διαστήματα. |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται γραμμές προόδου στις επιλεγμένες ημερομηνίες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν θα εμφανίζονται γραμμές προόδου στις επιλεγμένες ημερομηνίες. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Ορίζει τη γραμματοσειρά που χρησιμοποιείται για την ετικέτα της γραμμής προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | η γραμματοσειρά που χρησιμοποιείται για την ετικέτα της γραμμής προόδου. |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


Ορίζει το χρώμα της γραμμής για την τρέχουσα γραμμή προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | το χρώμα γραμμής για την τρέχουσα γραμμή προόδου. |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


Ορίζει το μοτίβο γραμμής της τρέχουσας γραμμής προόδου. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το μοτίβο γραμμής της τρέχουσας γραμμής προόδου. |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


Ορίζει το χρώμα της άλλης γραμμής προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | το χρώμα της άλλης γραμμής προόδου. |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


Ορίζει το μοτίβο γραμμής για την άλλη γραμμή προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το μοτίβο γραμμής για την άλλη γραμμή προόδου. |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


Ορίζει το χρώμα του άλλου σημείου προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | το χρώμα του άλλου σημείου προόδου. |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


Ορίζει το σχήμα του σημείου προόδου της άλλης γραμμής προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το σχήμα σημείου προόδου της άλλης γραμμής προόδου. |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


Ορίζει το χρώμα του σημείου προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | το χρώμα του σημείου προόδου. |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


Ορίζει το σχήμα σημείου προόδου. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το σχήμα σημείου προόδου. |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


Ορίζει το επαναλαμβανόμενο διάστημα. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | το επαναλαμβανόμενο διάστημα. |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν θα εμφανίζεται η ημερομηνία για κάθε γραμμή προόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν θα εμφανίζεται η ημερομηνία για κάθε γραμμή προόδου. |

