---
title: "OutlineMaskCollection.Remove"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineMaskCollection 方法。移除此集合中指定对象的第一次出现"
type: docs
weight: 110
url: /zh/net/aspose.tasks/outlinemaskcollection/remove/
---
## OutlineMaskCollection.Remove method

从此集合中移除特定对象的第一次出现。

```csharp
public bool Remove(OutlineMask item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | OutlineMask | 要删除的指定对象。 |

### 返回值

如果成功从此集合中删除指定对象则返回 true；否则返回 false。

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

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


