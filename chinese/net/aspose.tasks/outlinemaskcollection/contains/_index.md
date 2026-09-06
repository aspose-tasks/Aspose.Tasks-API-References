---
title: "OutlineMaskCollection.Contains"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineMaskCollection 方法。若在此集合中找到指定项则返回 true，否则返回 false。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/outlinemaskcollection/contains/
---
## OutlineMaskCollection.Contains method

如果在此集合中找到指定项则返回 true；否则返回 false。

```csharp
public bool Contains(OutlineMask item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | OutlineMask | 要查找的指定项。 |

### 返回值

如果在此集合中找到指定项则返回 true；否则返回 false。

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


