---
title: "OutlineMask.Level"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineMask 属性。获取或设置掩码的级别"
type: docs
weight: 30
url: /zh/net/aspose.tasks/outlinemask/level/
---
## OutlineMask.Level property

获取或设置掩码的级别。

```csharp
public int Level { get; set; }
```

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

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


