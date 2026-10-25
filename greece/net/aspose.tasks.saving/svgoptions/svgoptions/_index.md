---
title: "SvgOptions.SvgOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής SvgOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης SvgOptions που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή SVG."
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`SvgOptions`](../) που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή SVG.

```csharp
public SvgOptions()
```

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

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


