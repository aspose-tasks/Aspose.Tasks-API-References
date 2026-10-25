---
title: "Gridline.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Gridline. Επιστρέφει μια σημαία που υποδεικνύει εάν αυτό το αντικείμενο είναι ίσο με το καθορισμένο αντικείμενο."
type: docs
weight: 50
url: /el/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

Επιστρέφει μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | το καθορισμένο αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα των γραμμών πλέγματος.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// Η ισότητα των γραμμών πλέγματος ελέγχεται έναντι του τύπου γραμμής πλέγματος.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// αλλάξτε τον τύπο
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### Δείτε επίσης

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


