---
title: "Enum WorkGroupType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.WorkGroupType enum. Menentukan tipe grup kerja."
type: docs
weight: 3620
url: /id/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Menentukan tipe grup kerja.

```csharp
public enum WorkGroupType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Default | `0` | Menunjukkan tipe grup kerja Default. |
| None | `1` | Menunjukkan tipe grup kerja None. |
| Email | `2` | Menunjukkan tipe grup kerja Email. |
| Web | `3` | Menunjukkan tipe grup kerja Web. |

## Contoh

Menampilkan cara mengatur grup kerja sumber daya.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


