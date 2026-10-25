---
title: "OutlineMaskCollection.IndexOf"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineMaskCollection 메서드. 지정된 항목의 인덱스를 이 컬렉션에서 결정합니다"
type: docs
weight: 90
url: /ko/net/aspose.tasks/outlinemaskcollection/indexof/
---
## OutlineMaskCollection.IndexOf method

이 컬렉션에서 지정된 항목의 인덱스를 결정합니다.

```csharp
public int IndexOf(OutlineMask item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | OutlineMask | 이 컬렉션에서 찾을 지정된 항목. |

### 반환 값

찾은 경우 지정된 항목의 인덱스; 찾지 못하면 -1.

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

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


