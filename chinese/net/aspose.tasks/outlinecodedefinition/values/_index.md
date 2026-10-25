---
title: "OutlineCodeDefinition.Values"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineCodeDefinition 属性。获取 OutlineValueCollection 对象。与此大纲代码关联的表格中的值"
type: docs
weight: 150
url: /zh/net/aspose.tasks/outlinecodedefinition/values/
---
## OutlineCodeDefinition.Values property

获取 OutlineValueCollection 对象。与此大纲代码关联的表的值。

```csharp
public OutlineValueCollection Values { get; }
```

## 示例

展示如何创建新的大纲代码。

```csharp
var project = new Project(DataDir + "project.mpp");

// 定义大纲代码及其大纲掩码
var code1 = new OutlineCodeDefinition();
code1.Alias = "New task outline code1";
code1.FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString();
code1.FieldName = "Outline Code1";
var mask = new OutlineMask();
mask.Separator = "+";
mask.Level = 1;
mask.Type = MaskType.Numbers;
code1.Masks.Add(mask);

// 添加大纲值
var value = new OutlineValue();
value.Description = "Value description";
value.ValueId = 1;
value.Value = "123456";
value.Type = OutlineValueType.Number;
code1.Values.Add(value);

// 将大纲代码添加到项目
project.OutlineCodes.Add(code1);

// 定义大纲代码及其大纲掩码
var code2 = new OutlineCodeDefinition();
code2.Alias = "New rsc outline code2";
code2.FieldId = ((int)ExtendedAttributeResource.OutlineCode2).ToString();
code2.FieldName = "Outline Code2";
var mask2 = new OutlineMask();
mask2.Separator = "/";
mask2.Level = 1;
mask2.Type = MaskType.Numbers;
code2.Masks.Add(mask2);

// 添加大纲值
var value2 = new OutlineValue();
value2.Description = "Value2 description";
value2.ValueId = 2;
value2.Value = "987654";
value2.Type = OutlineValueType.Number;
code2.Values.Add(value2);

// 将大纲代码添加到项目
project.OutlineCodes.Add(code2);

project.Save(OutDir + "Updated_project_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [OutlineValueCollection](../../outlinevaluecollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


