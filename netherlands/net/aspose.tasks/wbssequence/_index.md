---
title: "Enum WBSSequence"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WBSSequence enum. Specificeert de volgorde voor WBSCodeMask."
type: docs
weight: 3520
url: /nl/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

Specificeert de volgorde voor WBSCodeMask

```csharp
public enum WBSSequence
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| OrderedNumbers | `0` | Geeft de cijfers WBS‑volgorde aan. |
| OrderedUppercaseLetters | `1` | Geeft de hoofdletters WBS‑volgorde aan. |
| OrderedLowercaseLetters | `2` | Geeft de kleine letters WBS‑volgorde aan. |
| UnorderedCharacters | `3` | Geeft de ongeordende tekens WBS‑volgorde aan. |

## Voorbeelden

Toont hoe WBS‑volgordes in te stellen.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


