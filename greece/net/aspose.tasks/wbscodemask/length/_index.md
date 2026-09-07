---
title: "WBSCodeMask.Length"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα WBSCodeMask. Λαμβάνει ή ορίζει τον αριθμό των χαρακτήρων της συμβολοσειράς κώδικα"
type: docs
weight: 20
url: /el/net/aspose.tasks/wbscodemask/length/
---
## WBSCodeMask.Length property

Λαμβάνει ή ορίζει τον αριθμό των χαρακτήρων της συμβολοσειράς κώδικα.

```csharp
public byte Length { get; set; }
```

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

* class [WBSCodeMask](../)
* namespace [Aspose.Tasks](../../wbscodemask/)
* assembly [Aspose.Tasks](../../../)


