---
title: "Κλάση PageLegend"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.PageLegend. Αντιπροσωπεύει ένα υπόμνημα σελίδας που χρησιμοποιείται για εκτύπωση έργου."
type: docs
weight: 3210
url: /el/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Αναπαριστά ένα υπόμνημα σελίδας που χρησιμοποιείται για την εκτύπωση του έργου.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PageLegend](pagelegend/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Λαμβάνει ή ορίζει την κεντραρισμένη εικόνα που θα εμφανίζεται στο γονικό στοιχείο. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Λαμβάνει ή ορίζει το εμφανιζόμενο μέγεθος της κεντρικής εικόνας. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Λαμβάνει ή ορίζει το κεντραρισμένο κείμενο που θα εμφανίζεται στο γονικό στοιχείο. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Λαμβάνει ή ορίζει την αριστερά ευθυγραμμισμένη εικόνα που θα εμφανίζεται στο γονικό στοιχείο. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Λαμβάνει ή ορίζει το εμφανιζόμενο μέγεθος της αριστερής εικόνας. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Λαμβάνει ή ορίζει το αριστερά ευθυγραμμισμένο κείμενο που θα εμφανίζεται στο γονικό στοιχείο. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Λαμβάνει ή ορίζει τις σελίδες στις οποίες εμφανίζεται το υπόμνημα. Μπορεί να είναι μία από τις τιμές της απαρίθμησης [`Legend`](../legend/). |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Λαμβάνει ή ορίζει την δεξιά ευθυγραμμισμένη εικόνα που θα εμφανίζεται στο γονικό στοιχείο. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Λαμβάνει ή ορίζει το εμφανιζόμενο μέγεθος της δεξιάς εικόνας. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Λαμβάνει ή ορίζει το δεξιά ευθυγραμμισμένο κείμενο που θα εμφανίζεται στο γονικό στοιχείο. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Λαμβάνει ή ορίζει το πλάτος του αριστερού τμήματος (που περιέχει το όνομα και την ημερομηνία του έργου από προεπιλογή) του υπομνήματος σε εκατοστά. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις πληροφορίες του υπομνήματος σελίδας.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Ας διαβάσουμε τις πληροφορίες του υπομνήματος σελίδας.
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// Επίσης υποστηρίζεται η τροποποίηση ενός υπομνήματος.
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


