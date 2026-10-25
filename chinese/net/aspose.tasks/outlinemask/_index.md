---
title: "类 OutlineMask"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OutlineMask 类。表示定义大纲代码格式的掩码的四个元素"
type: docs
weight: 1190
url: /zh/net/aspose.tasks/outlinemask/
---
## OutlineMask class

表示定义大纲代码格式的掩码的四个元素。

```csharp
public class OutlineMask
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [OutlineMask](outlinemask/)() | 初始化 `OutlineMask` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | 获取或设置大纲代码值的最大长度（以字符计）。如果未定义长度，则为 0。 |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | 获取或设置掩码的级别。 |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | 获取或设置代码值的分隔符。 |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | 获取或设置掩码的类型。 |

## 示例

展示如何使用大纲掩码。

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// 设置掩码的类型
mask.Type = MaskType.Characters;

// 设置代码值的分隔符
mask.Separator = "/";

// 设置掩码的级别
mask.Level = 1;

// 设置大纲代码值的最大长度（字符数）。如果未定义长度，则为 0。
mask.Length = 2;

// 将掩码添加到定义中
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


