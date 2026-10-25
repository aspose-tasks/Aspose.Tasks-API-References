---
title: "OutlineValue.IsCollapsed"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineValue 속성. 개요 값이 축소되었는지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/outlinevalue/iscollapsed/
---
## OutlineValue.IsCollapsed property

개요 값이 축소되었는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool IsCollapsed { get; set; }
```

## 비고

이것은 MS Project 2010 속성에 대한 새로운 기능입니다.

## 예제

개요 값 작업 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// 개요 값을 생성합니다
var value = new OutlineValue();

// 실제 값을 설정합니다
value.Value = "Text value 1";

// 프로젝트 내 개요 코드 값의 고유 ID를 설정합니다
value.ValueId = 1;

// 전체 프로젝트에서 이 값을 다른 값들과 구분하는 GUID를 가져옵니다
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// 개요 코드 유형을 설정합니다
value.Type = OutlineValueType.Text;

// 개요 값의 설명을 설정합니다
value.Description = "Text value descr 1";

// 개요 값이 축소되었는지 여부를 나타내는 값을 설정합니다
value.IsCollapsed = false;

// 상위 값 ID를 확인합니다
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// 기간이 포함된 개요 값을 생성합니다
var value2 = new OutlineValue();

// 기간 값을 설정합니다
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// 프로젝트 내 개요 코드 값의 고유 ID를 설정합니다
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### 또 보기

* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)


