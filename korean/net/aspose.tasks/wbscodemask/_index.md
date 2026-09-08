---
title: "클래스 WBSCodeMask"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WBSCodeMask 클래스. WBS 코드 마스크를 나타냅니다."
type: docs
weight: 3500
url: /ko/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

WBS 코드 마스크를 나타냅니다.

```csharp
public class WBSCodeMask
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | `WBSCodeMask` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | 코드 문자열의 문자 수를 가져오거나 설정합니다. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | 마스크 수준을 가져옵니다. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | 코드 문자열의 구분자를 가져오거나 설정합니다. 기본값은 Period입니다. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | 코드 문자열의 문자 유형을 가져오거나 설정합니다. |

## 예제

WBS 코드 마스크를 만드는 방법을 보여줍니다.

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

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


