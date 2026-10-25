---
title: "Class OutlineValue"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OutlineValue 클래스. 개요 값을 나타냅니다."
type: docs
weight: 1210
url: /ko/net/aspose.tasks/outlinevalue/
---
## OutlineValue class

아웃라인 값을 나타냅니다.

```csharp
public class OutlineValue
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [OutlineValue](outlinevalue/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Description](../../aspose.tasks/outlinevalue/description/) { get; set; } | 개요 값의 설명을 가져오거나 설정합니다. |
| [DurationValue](../../aspose.tasks/outlinevalue/durationvalue/) { get; set; } | Type이 Duration인 경우 지속 시간을 가져오거나 설정합니다. |
| [IsCollapsed](../../aspose.tasks/outlinevalue/iscollapsed/) { get; set; } | 개요 값이 축소되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ParentValueId](../../aspose.tasks/outlinevalue/parentvalueid/) { get; set; } | 개요 코드의 상위 노드 ID를 가져오거나 설정합니다. |
| [Type](../../aspose.tasks/outlinevalue/type/) { get; set; } | 개요 코드 유형을 가져오거나 설정합니다. |
| [Value](../../aspose.tasks/outlinevalue/value/) { get; set; } | 실제 값을 가져오거나 설정합니다. |
| [ValueGuid](../../aspose.tasks/outlinevalue/valueguid/) { get; } | 전체 프로젝트에서 이 값을 다른 값들과 구분하는 GUID를 가져옵니다. |
| [ValueId](../../aspose.tasks/outlinevalue/valueid/) { get; set; } | 프로젝트 내 개요 코드 값의 고유 ID를 가져오거나 설정합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


