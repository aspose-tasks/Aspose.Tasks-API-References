---
title: "클래스 OutlineMaskCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OutlineMaskCollection 클래스. OutlineMask 객체의 컬렉션을 나타냅니다"
type: docs
weight: 1200
url: /ko/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

[`OutlineMask`](../outlinemask/) 객체의 컬렉션을 나타냅니다.

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환하거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | 이 컬렉션에서 지정된 항목의 인덱스를 결정합니다. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | 지정된 인덱스에 지정된 항목을 삽입합니다. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | 지정된 인덱스의 항목을 제거합니다. |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


