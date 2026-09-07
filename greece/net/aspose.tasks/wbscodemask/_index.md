---
title: "Κλάση WBSCodeMask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.WBSCodeMask. Αντιπροσωπεύει μάσκα κώδικα WBS"
type: docs
weight: 3500
url: /el/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

Αντιπροσωπεύει τη μάσκα κώδικα WBS.

```csharp
public class WBSCodeMask
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `WBSCodeMask`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των χαρακτήρων της συμβολοσειράς κώδικα. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Λαμβάνει το επίπεδο μάσκας. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Λαμβάνει ή ορίζει το διαχωριστικό της συμβολοσειράς κώδικα. Η προεπιλεγμένη τιμή είναι Period. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο χαρακτήρα της συμβολοσειράς κώδικα. |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε μάσκες κώδικα WBS.

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

var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

project.Recalculate();

Console.WriteLine("Number of WBS masks: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
var i = 0;
foreach (var cm in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("WBS Mask #{0}: Level->{1}", ++i, cm.Level);
}

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


