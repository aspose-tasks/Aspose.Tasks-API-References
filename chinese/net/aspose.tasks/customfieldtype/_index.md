---
title: "枚举 CustomFieldType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CustomFieldType 枚举。指定自定义字段的类型"
type: docs
weight: 380
url: /zh/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

指定自定义字段的类型。

```csharp
public enum CustomFieldType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Null | `0` | 指示空（Null）自定义字段类型。 |
| Cost | `1` | 指示成本自定义字段类型。 |
| Date | `2` | 指示日期自定义字段类型。 |
| Duration | `3` | 指示持续时间自定义字段类型。 |
| Finish | `4` | 指示完成自定义字段类型。 |
| Flag | `5` | 指示标志自定义字段类型。 |
| Number | `6` | 指示数字自定义字段类型。 |
| Start | `7` | 指示开始自定义字段类型。 |
| Text | `8` | 指示文本自定义字段类型。 |
| OutlineCode | `9` | 指示大纲代码自定义字段类型。 |
| RBS | `10` | 指示 RBS（资源分解结构）自定义字段类型。 |

## 示例

展示如何使用 &lt;see cref="CustomFieldType" /&gt;（CustomFieldType.Text）。

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// 处理定义...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


