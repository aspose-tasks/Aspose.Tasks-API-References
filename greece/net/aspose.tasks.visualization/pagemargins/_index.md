---
title: "Κλάση PageMargins"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.PageMargins. Αντιπροσωπεύει τα περιθώρια σελίδας για εκτύπωση"
type: docs
weight: 3230
url: /el/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Αναπαριστά τα περιθώρια σελίδας για εκτύπωση.

```csharp
public class PageMargins
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PageMargins](pagemargins/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Λαμβάνει ή ορίζει μια θέση όπου θα εκτυπωθούν τα περιγράμματα. Μπορεί να είναι μία από τις τιμές της αρίθμησης [`Border`](../border/). |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος του κάτω περιθωρίου σε εκατοστά. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος του αριστερού περιθωρίου σε εκατοστά. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος του δεξιού περιθωρίου σε εκατοστά. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος του πάνω περιθωρίου σε εκατοστά. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τα περιθώρια σελίδας.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// επιτρέπει την τροποποίηση της προεπιλεγμένης προβολής
var margins = project.DefaultView.PageInfo.Margins;

// επιτρέπει την τροποποίηση των περιθωρίων
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


