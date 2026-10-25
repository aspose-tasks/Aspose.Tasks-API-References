---
title: "Project.WBSCodeDefinition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 프로젝트의 WBS 코드 정의를 가져오거나 설정합니다"
type: docs
weight: 1030
url: /ko/net/aspose.tasks/project/wbscodedefinition/
---
## Project.WBSCodeDefinition property

프로젝트에 대한 WBS 코드 정의를 가져오거나 설정합니다.

```csharp
public WBSCodeDefinition WBSCodeDefinition { get; set; }
```

## 예제

WBS 코드를 추가하는 방법을 보여줍니다.

```csharp
var project = new Project
{
    WBSCodeDefinition = new WBSCodeDefinition()
};
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask
{
    Length = 2,
    Separator = "-",
    Sequence = WBSSequence.OrderedNumbers
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask
{
    Length = 1,
    Separator = "-",
    Sequence = WBSSequence.OrderedUppercaseLetters
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### 또 보기

* class [WBSCodeDefinition](../../wbscodedefinition/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


