---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageSettings. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα προσαρμοστεί η εκτύπωση στο καθορισμένο ποσοστό PercentOfNormalSize του κανονικού μεγέθους"
type: docs
weight: 20
url: /el/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα προσαρμοστεί η εκτύπωση στο καθορισμένο ποσοστό ([`PercentOfNormalSize`](../percentofnormalsize/)) του κανονικού μεγέθους.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## Παρατηρήσεις

Δεν είναι αποτελεσματικό όταν το έργο αποδίδεται σε μορφή HTML.

## Παραδείγματα

Εμφανίζει πώς να αποδοθεί η προβολή με τον καθορισμένο συντελεστή κλίμακας.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// ορίστε μια τιμή που υποδεικνύει ότι η προβολή πρέπει να κλιμακωθεί χρησιμοποιώντας τον καθορισμένο συντελεστή κλίμακας
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// καθορίστε τον συντελεστή κλίμακας
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### Δείτε επίσης

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


