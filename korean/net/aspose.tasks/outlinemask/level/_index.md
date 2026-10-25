---
title: "OutlineMask.Level"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineMask 속성. 마스크의 레벨을 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/outlinemask/level/
---
## OutlineMask.Level property

마스크의 레벨을 가져오거나 설정합니다.

```csharp
public int Level { get; set; }
```

## 예제

개요 마스크를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// 마스크 유형을 설정합니다
mask.Type = MaskType.Characters;

// 코드 값의 구분자를 설정합니다
mask.Separator = "/";

// 마스크 수준을 설정합니다
mask.Level = 1;

// 개요 코드 값의 최대 길이(문자 수)를 설정합니다. 길이가 정의되지 않은 경우 0입니다.
mask.Length = 2;

// 정의에 마스크를 추가합니다
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### 또 보기

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


