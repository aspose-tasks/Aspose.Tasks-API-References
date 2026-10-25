---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectView. Περιλαμβάνει στήλες πόρου UID, όνομα, τύπο, υλικό, ετικέτα, αρχικά, ομάδα, μέγιστες μονάδες, τυπικό ποσοστό, υπερωριακό ποσοστό, κόστος ανά χρήση, συσσωμάτωση στο βασικό ημερολόγιο και κώδικα"
type: docs
weight: 40
url: /el/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Περιλαμβάνει στήλες Uid, όνομα πόρου, τύπο, ετικέτα υλικού, αρχικά, ομάδα, μέγιστες μονάδες, τυπική τιμή, τιμή υπερωρίας, κόστος ανά χρήση, συσσωμάτωση, βασικό ημερολόγιο και κώδικα πόρου.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Τιμή Επιστροφής

μια προβολή που περιέχει μια λίστα των [`ResourceViewColumn`](../../resourceviewcolumn/).

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο με προβολή φύλλου πόρων.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### Δείτε επίσης

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


