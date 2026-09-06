---
title: "OutlineMaskCollection.RemoveAt"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineMaskCollection 方法。移除指定索引处的项"
type: docs
weight: 120
url: /zh/net/aspose.tasks/outlinemaskcollection/removeat/
---
## OutlineMaskCollection.RemoveAt method

在指定索引处移除一项。

```csharp
public void RemoveAt(int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | Int32 | 要在其移除项的指定零基索引。 |

## 示例

展示如何使用大纲掩码集合。

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// 清除大纲掩码
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

// 插入一个错误的掩码
outline.Masks.Insert(0, maskWrong);

// 通过使用集合的索引访问编辑掩码
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// 通过索引移除错误的掩码
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// 遍历掩码
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

### 另见

* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


