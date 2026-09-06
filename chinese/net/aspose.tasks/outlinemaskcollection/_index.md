---
title: "类 OutlineMaskCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OutlineMaskCollection 类。表示 OutlineMask 对象的集合"
type: docs
weight: 1200
url: /zh/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

表示 [`OutlineMask`](../outlinemask/) 对象的集合。

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | 返回或设置指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | 确定此集合中指定项的索引。 |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | 在指定索引处插入指定项。 |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | 从此集合中移除特定对象的第一次出现。 |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | 在指定索引处移除一项。 |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


