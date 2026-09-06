---
title: "OutlineValue.Value"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineValue 属性。获取或设置实际值"
type: docs
weight: 70
url: /zh/net/aspose.tasks/outlinevalue/value/
---
## OutlineValue.Value property

获取或设置实际值。

```csharp
public string Value { get; set; }
```

## 示例

展示如何使用大纲值。

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// 创建大纲值
var value = new OutlineValue();

// 设置实际值
value.Value = "Text value 1";

// 设置项目中大纲代码值的唯一 Id
value.ValueId = 1;

// 获取在整个项目中标识此值的 GUID
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// 设置大纲代码类型
value.Type = OutlineValueType.Text;

// 设置大纲值的描述
value.Description = "Text value descr 1";

// 设置指示大纲值是否折叠的值
value.IsCollapsed = false;

// 检查父值 Id
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// 创建带持续时间的大纲值
var value2 = new OutlineValue();

// 设置持续时间值
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// 设置项目中大纲代码值的唯一 Id
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### 另见

* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)


