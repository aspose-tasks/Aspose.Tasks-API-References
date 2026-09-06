---
title: "تعداد CustomFieldType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.CustomFieldType. يحدد نوع الحقل المخصص"
type: docs
weight: 380
url: /ar/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

يحدد نوع الحقل المخصص.

```csharp
public enum CustomFieldType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Null | `0` | يشير إلى نوع الحقل المخصص Null. |
| Cost | `1` | يشير إلى نوع الحقل المخصص Cost. |
| Date | `2` | يشير إلى نوع الحقل المخصص Date. |
| Duration | `3` | يشير إلى نوع الحقل المخصص Duration. |
| Finish | `4` | يشير إلى نوع الحقل المخصص Finish. |
| Flag | `5` | يشير إلى نوع الحقل المخصص Flag. |
| Number | `6` | يشير إلى نوع الحقل المخصص Number. |
| Start | `7` | يشير إلى نوع الحقل المخصص Start. |
| Text | `8` | يشير إلى نوع الحقل المخصص Text. |
| OutlineCode | `9` | يشير إلى نوع الحقل المخصص Outline Code. |
| RBS | `10` | يشير إلى نوع الحقل المخصص RBS (Resource Breakdown Structure). |

## الأمثلة

يظهر كيفية استخدام &lt;see cref=\"CustomFieldType\" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// العمل مع التعريفات...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


