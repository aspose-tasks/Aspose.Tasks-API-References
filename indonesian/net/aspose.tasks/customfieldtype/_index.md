---
title: "Enum CustomFieldType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.CustomFieldType enum. Menentukan jenis bidang khusus"
type: docs
weight: 380
url: /id/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Menentukan tipe bidang khusus.

```csharp
public enum CustomFieldType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Null | `0` | Menunjukkan tipe bidang khusus Null. |
| Cost | `1` | Menunjukkan tipe bidang khusus Cost. |
| Date | `2` | Menunjukkan tipe bidang khusus Date. |
| Duration | `3` | Menunjukkan tipe bidang khusus Duration. |
| Finish | `4` | Menunjukkan tipe bidang khusus Finish. |
| Flag | `5` | Menunjukkan tipe bidang khusus Flag. |
| Number | `6` | Menunjukkan tipe bidang khusus Number. |
| Start | `7` | Menunjukkan tipe bidang khusus Start. |
| Text | `8` | Menunjukkan tipe bidang khusus Text. |
| OutlineCode | `9` | Menunjukkan tipe bidang khusus Outline Code. |
| RBS | `10` | Menunjukkan tipe bidang khusus RBS (Resource Breakdown Structure). |

## Contoh

Menampilkan cara menggunakan &lt;see cref=\"CustomFieldType\" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// bekerja dengan definisi...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


