---
title: "Κλάση WBSCodeDefinition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WBSCodeDefinition κλάση. Αντιπροσωπεύει έναν ορισμό κώδικα WBS"
type: docs
weight: 3490
url: /el/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Αντιπροσωπεύει έναν ορισμό κώδικα WBS.

```csharp
public class WBSCodeDefinition
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `WBSCodeDefinition`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | Λαμβάνει τη συλλογή των αντικειμένων WBSCodeMask. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Λαμβάνει ή ορίζει το πρόθεμα κώδικα του έργου. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα δημιουργηθεί κώδικας WBS για νέα εργασία. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα επαληθευτεί η μοναδικότητα των νέων κωδίκων WBS. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε μάσκες κώδικα WBS.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask();
mask.Length = 2;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask();
mask.Length = 1;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


