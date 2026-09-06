---
title: "枚举 MaskType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.MaskType 枚举。指定掩码的类型"
type: docs
weight: 1000
url: /zh/net/aspose.tasks/masktype/
---
## MaskType enumeration

指定掩码的类型。

```csharp
public enum MaskType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Null | `0` | 指示空（Null）掩码类型。 |
| Numbers | `1` | 指示数字掩码类型。 |
| UpperCaseLetters | `2` | 指示大写字母掩码类型。 |
| LowerCaseLetters | `3` | 指示小写字母掩码类型。 |
| Characters | `4` | 指示字符掩码类型。 |
| Val4 | `5` | 指示成本查找掩码类型。 |
| Val5 | `6` | 指示日期查找掩码类型。 |
| Val6 | `7` | 指示持续时间查找掩码类型。 |
| Val7 | `8` | 指示数字查找掩码类型。 |
| Val8 | `9` | 指示标志查找掩码类型。 |
| Val9 | `10` | 指示完成日期查找掩码类型。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


