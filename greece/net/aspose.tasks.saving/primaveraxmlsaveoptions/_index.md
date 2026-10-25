---
title: "Κλάση PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Saving.PrimaveraXmlSaveOptions. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε μορφή Primavera xml"
type: docs
weight: 2160
url: /el/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε μορφή Primavera xml.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `PrimaveraXmlSaveOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα αποθηκευτεί μια ριζική εργασία ή όχι. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που αποδίδονται στα γραφήματα Gantt, Φύλλο Εργασιών και Χρήση Εργασιών. |

## Παραδείγματα

Δείχνει πώς να εξάγετε στο αρχείο Primavera XML.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Δείτε επίσης

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


