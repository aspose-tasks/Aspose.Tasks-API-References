---
title: "类 OutlineCodeDefinition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OutlineCodeDefinition 类。表示大纲代码定义。"
type: docs
weight: 1170
url: /zh/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

表示大纲代码定义。

```csharp
public sealed class OutlineCodeDefinition
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | 初始化 `OutlineCodeDefinition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | 获取或设置自定义大纲代码的别名。 |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | 获取或设置一个值，指示新代码是否必须具有所有层级。企业代码不支持此功能。 |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | 获取或设置一个值，指示自定义大纲代码是否为企业自定义大纲代码。 |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | 获取或设置对另一个自定义字段的引用，该字段的别名为此大纲代码定义。 |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | 获取或设置大纲代码的字段编号。 |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | 获取或设置自定义大纲代码的名称。 |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | 获取或设置大纲代码的 Guid。 |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | 获取或设置一个值，指示此大纲代码字段中指定的值是否必须为叶子值。 |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | 获取 OutlineMaskCollection 对象。定义大纲代码掩码的条目表。只读 [`OutlineMaskCollection`](../outlinemaskcollection/) 实例。 |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | 获取或设置一个值，指示指定的值是否必须来自值表。 |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | 获取或设置自定义大纲代码别名的拼音发音。 |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | 获取或设置一个值，指示自定义大纲代码是否可以在 Microsoft Project 的资源替换向导中使用。 |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | 获取或设置一个值，指示是否必须显示此大纲代码的缩进。 |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | 获取 OutlineValueCollection 对象。与此大纲代码关联的表的值。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


