---
title: "열거형 WBSSequence"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WBSSequence 열거형. WBSCodeMask에 대한 순서를 지정합니다."
type: docs
weight: 3520
url: /ko/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

WBSCodeMask에 대한 순서를 지정합니다.

```csharp
public enum WBSSequence
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| OrderedNumbers | `0` | 숫자 WBS 순서를 나타냅니다. |
| OrderedUppercaseLetters | `1` | 대문자 WBS 순서를 나타냅니다. |
| OrderedLowercaseLetters | `2` | 소문자 WBS 순서를 나타냅니다. |
| UnorderedCharacters | `3` | 정렬되지 않은 문자 WBS 순서를 나타냅니다. |

## 예제

WBS 순서를 설정하는 방법을 보여줍니다.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


