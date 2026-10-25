---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "UsageView ιδιότητα. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα εμφανιστούν σύντομα ονόματα κεφαλίδων λεπτομερειών ή όχι"
type: docs
weight: 40
url: /el/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται σύντομες ονομασίες κεφαλίδας λεπτομερειών ή όχι.

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
```

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

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


