---
title: "Enum WBSSequence"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WBSSequence enum. WBSCodeMask के लिए अनुक्रम निर्दिष्ट करता है।"
type: docs
weight: 3520
url: /hi/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

WBSCodeMask के लिए क्रम को निर्दिष्ट करता है

```csharp
public enum WBSSequence
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| OrderedNumbers | `0` | संख्याओं का WBS अनुक्रम दर्शाता है। |
| OrderedUppercaseLetters | `1` | बड़े अक्षरों का WBS अनुक्रम दर्शाता है। |
| OrderedLowercaseLetters | `2` | छोटे अक्षरों का WBS अनुक्रम दर्शाता है। |
| UnorderedCharacters | `3` | अव्यवस्थित अक्षरों का WBS अनुक्रम दर्शाता है। |

## उदाहरण

WBS अनुक्रम सेट करने का तरीका दिखाता है।

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

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


