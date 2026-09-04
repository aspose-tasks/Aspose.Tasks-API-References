---
title: "Κλίμακα χρόνου"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Ορίζει επιλογές που καθορίζουν πώς θα αποδοθεί η κλίμακα χρόνου στις προβολές Gantt Chart Task Usage ή Resource Usage όταν το έργο εξάγεται σε γραφική μορφή."
type: docs
weight: 323
url: /el/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Ορίζει επιλογές που καθορίζουν πώς να αποδοθεί η κλίμακα χρόνου σε προβολές Gantt Chart, Task Usage ή Resource Usage όταν το έργο εξάγεται σε γραφική μορφή.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [Days](#Days) | Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το ελάχιστο επίπεδο λεπτομέρειας είναι μία ημέρα. |
| [DefinedInView](#DefinedInView) | Χρησιμοποιήστε τις ρυθμίσεις κλίμακας χρόνου που ορίζονται στις ιδιότητες της προβολής του έργου: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το ελάχιστο επίπεδο λεπτομέρειας είναι ένας μήνας. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το επίπεδο λεπτομέρειας είναι το ένα τρίτο του μήνα. |
### Days {#Days}
```
public static final int Days
```


Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το ελάχιστο επίπεδο λεπτομέρειας είναι μία ημέρα.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Χρησιμοποιήστε τις ρυθμίσεις κλίμακας χρόνου που ορίζονται στις ιδιότητες της προβολής του έργου: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Ισχύει για μορφές που περιέχουν δεδομένα προβολής. Για παράδειγμα, έργα που διαβάζονται από μορφή MPP.

--------------------

Εάν οι ρυθμίσεις κλίμακας χρόνου δεν έχουν οριστεί για την προβολή, χρησιμοποιείται η προκαθορισμένη ρύθμιση Timescale.Days.

### Months {#Months}
```
public static final int Months
```


Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το ελάχιστο επίπεδο λεπτομέρειας είναι ένας μήνας.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το επίπεδο λεπτομέρειας είναι το ένα τρίτο του μήνα.

