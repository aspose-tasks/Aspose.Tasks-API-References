---
title: "WBSCodeDefinition 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.WBSCodeDefinition 클래스. WBS 코드 정의를 나타냅니다."
type: docs
weight: 3490
url: /ko/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

WBS 코드 정의를 나타냅니다.

```csharp
public class WBSCodeDefinition
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | `WBSCodeDefinition` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | WBSCodeMask 객체 컬렉션을 가져옵니다. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | 프로젝트 코드 접두사를 가져오거나 설정합니다. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | 새 작업에 대한 WBS 코드를 생성할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | 새 WBS 코드의 고유성을 확인할지 여부를 나타내는 값을 가져오거나 설정합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


