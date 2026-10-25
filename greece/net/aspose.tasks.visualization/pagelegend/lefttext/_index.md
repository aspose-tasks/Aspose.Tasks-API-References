---
title: "PageLegend.LeftText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageLegend. Λαμβάνει ή ορίζει το αριστερά ευθυγραμμισμένο κείμενο που θα εμφανίζεται στο υπόμνημα της σελίδας"
type: docs
weight: 50
url: /el/net/aspose.tasks.visualization/pagelegend/lefttext/
---
## PageLegend.LeftText property

Λαμβάνει ή ορίζει το αριστερά ευθυγραμμισμένο κείμενο που θα εμφανίζεται στο υπόμνημα της σελίδας.

```csharp
public string LeftText { get; set; }
```

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

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


