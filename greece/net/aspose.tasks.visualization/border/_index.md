---
title: "Enum Border"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.Border enum. Καθορίζει τον τύπο των περιγραμμάτων"
type: docs
weight: 2970
url: /el/net/aspose.tasks.visualization/border/
---
## Border enumeration

Καθορίζει τα σύνορα τύπου.

```csharp
public enum Border
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| NoBorder | `0` | Χωρίς περίγραμμα. |
| AroundEveryPage | `1` | Γύρω από κάθε σελίδα. |
| OutsidePages | `2` | Στις εξωτερικές σελίδες. |

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


