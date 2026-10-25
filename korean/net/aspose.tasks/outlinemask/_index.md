---
title: "클래스 OutlineMask"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OutlineMask 클래스. 마스크의 네 요소를 나타내며, 이는 개요 코드 형식을 정의합니다."
type: docs
weight: 1190
url: /ko/net/aspose.tasks/outlinemask/
---
## OutlineMask class

아웃라인 코드 형식을 정의하는 마스크의 네 요소를 나타냅니다.

```csharp
public class OutlineMask
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [OutlineMask](outlinemask/)() | `OutlineMask` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | 개요 코드 값의 최대 길이(문자 수)를 가져오거나 설정합니다. 길이가 정의되지 않은 경우 0입니다. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | 마스크의 레벨을 가져오거나 설정합니다. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | 코드 값의 구분자를 가져오거나 설정합니다. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | 마스크 유형을 가져오거나 설정합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


