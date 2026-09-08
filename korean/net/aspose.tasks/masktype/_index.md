---
title: "Enum MaskType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.MaskType 열거형. 마스크 유형을 지정합니다."
type: docs
weight: 1000
url: /ko/net/aspose.tasks/masktype/
---
## MaskType enumeration

마스크의 유형을 지정합니다.

```csharp
public enum MaskType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Null | `0` | Null 마스크 유형을 나타냅니다. |
| Numbers | `1` | Numbers 마스크 유형을 나타냅니다. |
| UpperCaseLetters | `2` | UpperCaseLetters 마스크 유형을 나타냅니다. |
| LowerCaseLetters | `3` | LowerCaseLetters 마스크 유형을 나타냅니다. |
| Characters | `4` | Characters 마스크 유형을 나타냅니다. |
| Val4 | `5` | Cost에 대한 Lookup 마스크 유형을 나타냅니다. |
| Val5 | `6` | Dates에 대한 Lookup 마스크 유형을 나타냅니다. |
| Val6 | `7` | Durations에 대한 Lookup 마스크 유형을 나타냅니다. |
| Val7 | `8` | Numbers에 대한 Lookup 마스크 유형을 나타냅니다. |
| Val8 | `9` | Flags에 대한 Lookup 마스크 유형을 나타냅니다. |
| Val9 | `10` | FinishDate에 대한 Lookup 마스크 유형을 나타냅니다. |

## 예제

outline 마스크 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// 개요 마스크 지우기
if (outline.Masks.Count > 0)
{
    if (!outline.Masks.IsReadOnly)
    {
        outline.Masks.Clear();
    }
}

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
var maskWrong = new OutlineMask();
maskWrong.Type = MaskType.Null;

outline.Masks.Add(mask);

// 잘못된 마스크를 삽입합니다.
outline.Masks.Insert(0, maskWrong);

// 컬렉션의 인덱스 접근을 사용하여 마스크를 편집합니다.
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// 인덱스로 잘못된 마스크를 제거합니다.
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// 마스크를 반복합니다.
foreach (var outlineMask in outline.Masks)
{
    Console.WriteLine("Length: " + outlineMask.Length);
    Console.WriteLine("Level: " + outlineMask.Level);
    Console.WriteLine("Separator: " + outlineMask.Separator);
    Console.WriteLine("Type: " + outlineMask.Type);
}

var otherProject = new Project(DataDir + "OutlineValues2010.mpp");

var otherOutline = otherProject.OutlineCodes[0];

var masks = new OutlineMask[outline.Masks.Count];
outline.Masks.CopyTo(masks, 0);

foreach (var maskToAdd in masks)
{
    if (!otherOutline.Masks.Contains(maskToAdd))
    {
        otherOutline.Masks.Add(maskToAdd);
    }
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


