---
title: "WBSCodeDefinition.GenerateWBSCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα WBSCodeDefinition. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα δημιουργηθεί κώδικας WBS για νέα εργασία"
type: docs
weight: 40
url: /el/net/aspose.tasks/wbscodedefinition/generatewbscode/
---
## WBSCodeDefinition.GenerateWBSCode property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα δημιουργηθεί κώδικας WBS για νέα εργασία.

```csharp
public bool GenerateWBSCode { get; set; }
```

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

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


