---
title: Enum CustomFieldType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CustomFieldType enum. Specifies the type of a custom field
type: docs
weight: 380
url: /net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Specifies the type of a custom field.

```csharp
public enum CustomFieldType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Null | `0` | Indicates Null custom field type. |
| Cost | `1` | Indicates Cost custom field type. |
| Date | `2` | Indicates Date custom field type. |
| Duration | `3` | Indicates Duration custom field type. |
| Finish | `4` | Indicates Finish custom field type. |
| Flag | `5` | Indicates Flag custom field type. |
| Number | `6` | Indicates Number custom field type. |
| Start | `7` | Indicates Start custom field type. |
| Text | `8` | Indicates Text custom field type. |
| OutlineCode | `9` | Indicates Outline Code custom field type. |
| RBS | `10` | Indicates RBS (Resource Breakdown Structure) custom field type. |

## Examples

Shows how to use &lt;see cref="CustomFieldType" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// work with definitions...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


