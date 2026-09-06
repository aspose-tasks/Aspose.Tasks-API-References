---
title: "OutlineCodeDefinition.FieldId"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineCodeDefinition 属性。获取或设置大纲代码的字段编号"
type: docs
weight: 60
url: /zh/net/aspose.tasks/outlinecodedefinition/fieldid/
---
## OutlineCodeDefinition.FieldId property

获取或设置大纲代码的字段编号。

```csharp
public string FieldId { get; set; }
```

## 示例

展示如何使用大纲代码定义。

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// 创建新的大纲代码定义
var outline = new OutlineCodeDefinition();

// 设置大纲代码的字段编号
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// 设置自定义大纲代码的名称
outline.FieldName = "Outline Code1";

// 设置大纲代码的 Guid
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// 设置一个值，指示此大纲代码字段中指定的值是否必须为叶子值
outline.LeafOnly = false;

// 设置自定义大纲代码的别名
outline.Alias = "My Outline Code";

// 设置自定义大纲代码别名的拼音发音
outline.PhoneticAlias = "Outline Code";

// 设置一个值，指示新代码是否必须包含所有层级。企业代码不适用。
outline.AllLevelsRequired = true;

// 设置一个值，指示自定义大纲代码是否为企业自定义大纲代码
outline.Enterprise = false;

// 设置对另一个自定义字段的引用，该字段的别名为此大纲代码定义
outline.EnterpriseOutlineCodeAlias = 0;

// 添加大纲掩码
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// 设置一个值，指示指定的值是否必须来自值表
outline.OnlyTableValuesAllowed = false;

// 设置一个值，指示自定义大纲代码是否可用
// 通过 Microsoft Project 中的资源替换向导
outline.ResourceSubstitutionEnabled = false;

// 设置一个值，指示是否必须显示此大纲代码的缩进。
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### 另见

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


