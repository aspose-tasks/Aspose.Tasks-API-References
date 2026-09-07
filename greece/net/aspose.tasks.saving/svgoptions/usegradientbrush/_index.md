---
title: "SvgOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SvgOptions. Καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου. Προς το παρόν η χρήση gradient brush δεν υποστηρίζεται για απόδοση σε SVG"
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

Καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου. Προς το παρόν η χρήση του gradient brush δεν υποστηρίζεται για απόδοση σε SVG.

```csharp
public override bool UseGradientBrush { get; set; }
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


