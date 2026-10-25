---
title: "Απαρίθμηση WBSSequence"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.WBSSequence. Καθορίζει τη σειρά για το WBSCodeMask"
type: docs
weight: 3520
url: /el/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

Καθορίζει τη σειρά για το WBSCodeMask

```csharp
public enum WBSSequence
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| OrderedNumbers | `0` | Δείχνει τη σειρά αριθμών WBS. |
| OrderedUppercaseLetters | `1` | Δείχνει τη σειρά κεφαλαίων γραμμάτων WBS. |
| OrderedLowercaseLetters | `2` | Δείχνει τη σειρά πεζών γραμμάτων WBS. |
| UnorderedCharacters | `3` | Δείχνει τη σειρά μη διατεταγμένων χαρακτήρων WBS. |

## Παραδείγματα

Δείχνει πώς να ορίσετε τις ακολουθίες WBS.

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


