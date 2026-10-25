---
title: "WBSCodeDefinition.VerifyUniqueness"
second_title: "Aspose.Tasks for .NET API 참조"
description: "WBSCodeDefinition 속성. 새 WBS 코드의 고유성을 확인할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/wbscodedefinition/verifyuniqueness/
---
## WBSCodeDefinition.VerifyUniqueness property

새 WBS 코드의 고유성을 확인할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool VerifyUniqueness { get; set; }
```

## 예제

WBS 코드 마스크를 추가하는 방법을 보여줍니다.

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

### 또 보기

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


