---
title: "PageMargins.Right"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageMargins. Λαμβάνει ή ορίζει το μέγεθος του δεξιού περιθωρίου σε εκατοστά"
type: docs
weight: 50
url: /el/net/aspose.tasks.visualization/pagemargins/right/
---
## PageMargins.Right property

Λαμβάνει ή ορίζει το μέγεθος του δεξιού περιθωρίου σε εκατοστά.

```csharp
public double Right { get; set; }
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

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


