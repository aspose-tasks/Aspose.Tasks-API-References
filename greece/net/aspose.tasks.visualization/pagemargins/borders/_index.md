---
title: "PageMargins.Borders"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "PageMargins ιδιότητα. Λαμβάνει ή ορίζει μια θέση όπου θα εκτυπωθούν τα περιθώρια. Μπορεί να είναι μία από τις τιμές της απαρίθμησης Border."
type: docs
weight: 20
url: /el/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Λαμβάνει ή ορίζει τη θέση όπου θα εκτυπωθούν τα περιγράμματα. Μπορεί να είναι μία από τις τιμές της απαρίθμησης [`Border`](../../border/).

```csharp
public Border Borders { get; set; }
```

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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


