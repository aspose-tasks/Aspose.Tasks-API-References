---
title: "Enum Timescale"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.Timescale enum. Ορίζει επιλογές που καθορίζουν πώς θα αποδοθεί η κλίμακα χρόνου σε προβολές Χρήσης Εργασιών ή Χρήσης Πόρων σε Διάγραμμα Gantt όταν το έργο εξάγεται σε γραφική μορφή."
type: docs
weight: 3430
url: /el/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Ορίζει επιλογές που καθορίζουν πώς να αποδοθεί η κλίμακα χρόνου σε προβολές Gantt Chart, Task Usage ή Resource Usage όταν το έργο εξάγεται σε μορφή γραφικού.

```csharp
public enum Timescale
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| DefinedInView | `0` | Χρησιμοποιήστε τις ρυθμίσεις κλίμακας χρόνου που ορίζονται στις ιδιότητες της προβολής του έργου: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Ισχύει για μορφές που περιέχουν δεδομένα προβολής. Για παράδειγμα, έργα που διαβάζονται από μορφή MPP. |
| Days | `1` | Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το ελάχιστο επίπεδο λεπτομέρειας είναι μία ημέρα. |
| ThirdsOfMonths | `10` | Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το επίπεδο λεπτομέρειας είναι ένα τρίτο του μήνα. |
| Months | `30` | Προκαθορισμένη διπλού επιπέδου κλίμακα χρόνου όπου το ελάχιστο επίπεδο λεπτομέρειας είναι ένας μήνας. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως αρχείο SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // ορίστε το <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" /> στο οποίο θα αποθηκευτεί το έγγραφο
                            PresentationFormat = PresentationFormat.GanttChart,

                            // ορίστε μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να χωρά το περιεχόμενό της
                            FitContent = true,

                            // ορίστε την ελάχιστη χρονική περίοδο για απόδοση. Η προεπιλεγμένη τιμή είναι <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου
                            // Προς το παρόν η χρήση του gradient brush δεν υποστηρίζεται για απόδοση σε SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


