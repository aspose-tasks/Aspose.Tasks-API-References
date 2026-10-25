---
title: "Κλάση UsageView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.UsageView κλάση. Αντιπροσωπεύει μια προβολή χρήσης σε ένα έργο"
type: docs
weight: 2650
url: /el/net/aspose.tasks/usageview/
---
## UsageView class

Αντιπροσωπεύει μια προβολή χρήσης σε ένα έργο.

```csharp
public abstract class UsageView : View
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Λαμβάνει ή ορίζει την ευθυγράμμιση των δεδομένων λεπτομερειών. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις του κάτω επιπέδου κλίμακας χρόνου της προβολής. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα εμφανίζεται η στήλη κεφαλίδας λεπτομερειών στην προβολή ή όχι. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται σύντομες ονομασίες κεφαλίδας λεπτομερειών ή όχι. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Λαμβάνει ή ορίζει ένα φίλτρο που χρησιμοποιείται σε μια μοναδική προβολή. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Λαμβάνει ή ορίζει μια ομάδα της μοναδικής προβολής. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το Microsoft Project επισημαίνει το φίλτρο για μια μοναδική προβολή. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις του μεσαίου επιπέδου κλίμακας χρόνου της προβολής. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα ενός αντικειμένου View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Λαμβάνει μια παρουσία της κλάσης [`PageInfo`](../view/pageinfo/). Αντιπροσωπεύει τα δεδομένα ρύθμισης σελίδας που υπάρχουν σε μορφή αρχείου mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Λαμβάνει το γονέα του αντικειμένου View. Μόνο για ανάγνωση [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα επαναλαμβάνεται η κεφαλίδα λεπτομερειών σε όλες τις γραμμές ανάθεσης ή όχι. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Λαμβάνει τον τύπο οθόνης για τη μοναδική προβολή. Μόνο για ανάγνωση [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το Microsoft Project εμφανίζει το όνομα της μοναδικής προβολής στη λίστα προβολών View ή Other Views στο Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Λαμβάνει ή ορίζει έναν πίνακα της μοναδικής προβολής. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις του ανώτερου επιπέδου κλίμακας χρόνου της προβολής. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | Λαμβάνει τον τύπο του στοιχείου στη μοναδική προβολή, όπως εργασίες ή πόρους. Μόνο για ανάγνωση [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Λαμβάνει το μοναδικό αναγνωριστικό μιας προβολής. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Λαμβάνει μια συλλογή αντικειμένων που αντιπροσωπεύουν τη θέση και την εμφάνιση του [`OleObject`](../oleobject/) στην προβολή. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Συγκρίνει την τρέχουσα παρουσία με ένα άλλο αντικείμενο του ίδιου τύπου και επιστρέφει έναν ακέραιο που υποδεικνύει εάν η τρέχουσα παρουσία προηγείται, ακολουθεί ή βρίσκεται στην ίδια θέση στη σειρά ταξινόμησης όπως το άλλο αντικείμενο. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης [`Resource`](../resource/). |

## Παραδείγματα

Δείχνει πώς να αποδίδεται η προβολή χρήσης εργασιών με λεπτομέρειες.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// πάρτε την προβολή
UsageView view = (TaskUsageView)project.DefaultView;

// η στήλη κεφαλίδας λεπτομερειών δεν θα εμφανιστεί
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// εμφάνιση στήλης κεφαλίδας λεπτομερειών
view.DisplayDetailsHeaderColumn = true;

// επανάληψη κεφαλίδας λεπτομερειών σε όλες τις γραμμές αναθέσεων
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Δείτε επίσης

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


