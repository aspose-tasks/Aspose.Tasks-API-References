---
title: "PageMargins.Bottom"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageMargins. Λαμβάνει ή ορίζει το μέγεθος του κάτω περιθωρίου σε εκατοστά"
type: docs
weight: 30
url: /el/net/aspose.tasks.visualization/pagemargins/bottom/
---
## PageMargins.Bottom property

Λαμβάνει ή ορίζει το μέγεθος του κάτω περιθωρίου σε εκατοστά.

```csharp
public double Bottom { get; set; }
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


