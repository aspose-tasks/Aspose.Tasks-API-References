---
title: "PrimaveraXmlSaveOptions.SkipSummaryAssignments"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraXmlSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν οι εκχωρήσεις πόρων σε εργασίες σύνοψης πρέπει να παραλειφθούν κατά την εξαγωγή"
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Παρατηρήσεις

Το λογισμικό Primavera δεν υποστηρίζει εκχωρήσεις πόρων σε εργασίες σύνοψης (WBS). Συνεπώς, η εξαγωγή τέτοιων εκχωρήσεων μπορεί να οδηγήσει σε ένα μη έγκυρο αρχείο σύμφωνα με το μοντέλο του Primavera. Εάν είναι true, οι εκχωρήσεις σε εργασίες σύνοψης παραλείπονται κατά την εξαγωγή. Εάν είναι false (η προεπιλεγμένη τιμή), θα εξαχθεί εξαίρεση εάν εντοπιστεί εκχώρηση σε εργασία σύνοψης κατά την εξαγωγή.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη σημαία SkipSummaryAssignments.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Το Primavera δεν υποστηρίζει εκχωρήσεις πόρων σε εργασίες σύνοψης.
// Έτσι, η εξαγωγή τέτοιων εκχωρήσεων σε μορφή Primavera μπορεί να οδηγήσει σε αρχεία που δεν μπορούν να εισαχθούν στο Primavera.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### Δείτε επίσης

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


