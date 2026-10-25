---
title: "GanttChartView"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια προβολή GanttChart."
type: docs
weight: 112
url: /el/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Αναπαριστά μια προβολή GanttChart.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [GanttChartView](../../com.aspose.tasks/ganttchartview). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Λαμβάνει μια λίστα αυτόματων φίλτρων της προβολής Gantt Chart. |
| [getBarRounding()](#getBarRounding--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι μπάρες στρογγυλοποιούνται στην πλησιέστερη ημέρα. |
| [getBarSize()](#getBarSize--) | Λαμβάνει το ύψος, σε σημεία, των μπάρων Gantt στο Gantt Chart. |
| [getBarStyles()](#getBarStyles--) | Λαμβάνει μια λίστα των γονικών (κοινών) στυλ μπαράς της προβολής Gantt Chart. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Λαμβάνει τις ρυθμίσεις του κάτω επιπέδου κλίμακας χρόνου της προβολής. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Λαμβάνει μια λίστα προσαρμοσμένων στυλ μπαράς ανά εργασία της προβολής Gantt Chart. |
| [getGridlines()](#getGridlines--) | Λαμβάνει μια λίστα των `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) της προβολής Gantt Chart. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι μπάρες συγκέντρωσης θα κρύβονται κατά την επέκταση της συνοπτικής εργασίας. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Λαμβάνει τις ρυθμίσεις του μεσαίου επιπέδου κλίμακας χρόνου της προβολής. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Λαμβάνει το χρώμα μη εργάσιμου χρόνου. |
| [getProgressLines()](#getProgressLines--) | Λαμβάνει τις γραμμές προόδου για την προβολή Gantt Chart. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι μπάρες στο Gantt Chart πρέπει να συγκεντρωθούν. |
| [getShowBarSplits()](#getShowBarSplits--) | Λαμβάνει μια τιμή που υποδεικνύει εάν τα διαχωρισμένα τμήματα εργασίας στο Gantt Chart πρέπει να εμφανίζονται. |
| [getShowDrawings()](#getShowDrawings--) | Λαμβάνει μια τιμή που υποδεικνύει εάν τα σχέδια στο Gantt Chart πρέπει να εμφανίζονται. |
| [getTableTextStyles()](#getTableTextStyles--) | Λαμβάνει μια λίστα των στυλ κειμένου πίνακα της προβολής Gantt Chart. |
| [getTextStyles()](#getTextStyles--) | Λαμβάνει μια λίστα του [TextStyle](../../com.aspose.tasks/textstyle) της προβολής Gantt Chart. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \\{@inheritDoc\\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Λαμβάνει τις ρυθμίσεις του άνω επιπέδου κλίμακας χρόνου της προβολής. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι μπάρες στρογγυλοποιούνται στην πλησιέστερη ημέρα. |
| [setBarSize(int value)](#setBarSize-int-) | Ορίζει το ύψος, σε σημεία, των μπάρων Gantt στο Gantt Chart. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ορίζει τις ρυθμίσεις του κάτω επιπέδου κλίμακας χρόνου της προβολής. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Ορίζει μια λίστα των `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) της προβολής Gantt Chart. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι ράβδοι συγκέντρωσης θα κρύβονται κατά την επέκταση της συνοπτικής εργασίας. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ορίζει τις ρυθμίσεις του ενδιάμεσου επιπέδου χρονοσειράς της προβολής. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Ορίζει το χρώμα μη εργάσιμου χρόνου. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Ορίζει τις γραμμές προόδου για την προβολή Gantt Chart. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι ράβδοι στο Gantt Chart πρέπει να συγκεντρώνονται. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι διαχωρισμοί εργασιών στο Gantt Chart πρέπει να εμφανίζονται. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν τα σχέδια στο Gantt Chart πρέπει να εμφανίζονται. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Ορίζει μια λίστα του [TextStyle](../../com.aspose.tasks/textstyle) της προβολής Gantt Chart. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \\{@inheritDoc\\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ορίζει τις ρυθμίσεις του ανώτερου επιπέδου χρονοσειράς της προβολής. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [GanttChartView](../../com.aspose.tasks/ganttchartview).

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Λαμβάνει μια λίστα αυτόματων φίλτρων της προβολής Gantt Chart.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι ράβδοι στρογγυλοποιούνται στην πλησιέστερη ημέρα. Η προεπιλεγμένη τιμή είναι True.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν οι ράβδοι στρογγυλοποιούνται στην πλησιέστερη ημέρα.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Λαμβάνει το ύψος, σε σημεία, των μπάρων Gantt στο Gantt Chart.

**Returns:**
int - το ύψος, σε σημεία, των ράβδων Gantt στο Gantt Chart.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Λαμβάνει μια λίστα των γονικών (κοινών) στυλ ράβδων της προβολής Gantt Chart. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - μια λίστα των γονικών (κοινών) στυλ ράβδων της προβολής Gantt Chart.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Λαμβάνει τις ρυθμίσεις του κατώτερου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Λαμβάνει μια λίστα των προσαρμοσμένων στυλ ράβδων για συγκεκριμένες εργασίες της προβολής Gantt Chart. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - μια λίστα των προσαρμοσμένων στυλ ράβδων για συγκεκριμένες εργασίες της προβολής Gantt Chart.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Λαμβάνει μια λίστα των `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) της προβολής Gantt Chart.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - μια λίστα των `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) της προβολής Gantt Chart.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι μπάρες συγκέντρωσης θα κρύβονται κατά την επέκταση της συνοπτικής εργασίας.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν οι ράβδοι συγκέντρωσης θα κρύβονται κατά την επέκταση της συνοπτικής εργασίας.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Λαμβάνει τις ρυθμίσεις του ενδιάμεσου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Λαμβάνει το χρώμα μη εργάσιμου χρόνου.

**Returns:**
java.awt.Color - χρώμα μη εργάσιμου χρόνου.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Λαμβάνει τις γραμμές προόδου για την προβολή Gantt Chart. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι μπάρες στο Gantt Chart πρέπει να συγκεντρωθούν.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν οι ράβδοι στο Gantt Chart πρέπει να συγκεντρώνονται.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν τα διαχωρισμένα τμήματα εργασίας στο Gantt Chart πρέπει να εμφανίζονται.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν οι διαχωρισμοί εργασιών στο Gantt Chart πρέπει να εμφανίζονται.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν τα σχέδια στο Gantt Chart πρέπει να εμφανίζονται.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν τα σχέδια στο Gantt Chart πρέπει να εμφανίζονται.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Λαμβάνει μια λίστα των στυλ κειμένου πίνακα της προβολής Gantt Chart. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - μια λίστα των στυλ κειμένου πίνακα της προβολής Gantt Chart.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Λαμβάνει μια λίστα του [TextStyle](../../com.aspose.tasks/textstyle) της προβολής Gantt Chart.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - μια λίστα του [TextStyle](../../com.aspose.tasks/textstyle) της προβολής Gantt Chart.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Λαμβάνει ένα ποσοστό για τη μείωση ή την αύξηση του διαστήματος μεταξύ των μονάδων στο επίπεδο χρονοσειράς.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Λαμβάνει τις ρυθμίσεις του ανώτερου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν οι μπαρές στρογγυλοποιούνται στην πιο κοντινή ημέρα. Η προεπιλεγμένη τιμή είναι True.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν οι μπαρές στρογγυλοποιούνται στην πιο κοντινή ημέρα. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Ορίζει το ύψος, σε σημεία, των μπάρων Gantt στο Gantt Chart.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το ύψος, σε μονάδες σημείου, των μπαρών Gantt στο Διάγραμμα Gantt. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Ορίζει τις ρυθμίσεις του κατώτερου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ρυθμίσεις του κατώτερου επιπέδου χρονοσειράς της προβολής. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Ορίζει μια λίστα των `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) της προβολής Gantt Chart.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | μια λίστα των `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) της προβολής Διάγραμμα Gantt. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν οι ράβδοι συγκέντρωσης θα κρύβονται κατά την επέκταση της συνοπτικής εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν οι μπαρές συγκέντρωσης θα κρυφτούν κατά την επέκταση της συνοπτικής εργασίας. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Ορίζει τις ρυθμίσεις του ενδιάμεσου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ρυθμίσεις του ενδιάμεσου επιπέδου χρονοσειράς της προβολής. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Ορίζει το χρώμα μη εργάσιμου χρόνου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | χρώμα μη εργάσιμου χρόνου. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Ορίζει γραμμές προόδου για την προβολή Διάγραμμα Gantt. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | γραμμές προόδου για την προβολή Διάγραμμα Gantt. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν οι ράβδοι στο Gantt Chart πρέπει να συγκεντρώνονται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν οι μπαρές στο Διάγραμμα Gantt πρέπει να συγκεντρωθούν. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν οι διαχωρισμοί εργασιών στο Gantt Chart πρέπει να εμφανίζονται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν τα διαχωρισμένα τμήματα εργασίας στο Διάγραμμα Gantt πρέπει να εμφανιστούν. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν τα σχέδια στο Gantt Chart πρέπει να εμφανίζονται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν τα σχέδια στο Διάγραμμα Gantt πρέπει να εμφανιστούν. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Ορίζει μια λίστα του [TextStyle](../../com.aspose.tasks/textstyle) της προβολής Gantt Chart.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | μια λίστα του [TextStyle](../../com.aspose.tasks/textstyle) της προβολής Διάγραμμα Gantt. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Ορίζει ένα ποσοστό για τη μείωση ή την αύξηση του διαστήματος μεταξύ των μονάδων στο επίπεδο χρονοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | \\{@inheritDoc\\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Ορίζει τις ρυθμίσεις του ανώτερου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ρυθμίσεις του ανώτερου επιπέδου χρονοσειράς της προβολής. |

