---
title: "Enum CostAccrualType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.CostAccrualType. Menentukan jenis biaya akrual"
type: docs
weight: 350
url: /id/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

Menentukan tipe biaya akrual.

```csharp
public enum CostAccrualType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Menunjukkan nilai undefined berarti bahwa bidang tidak didefinisikan dalam file proyek asli. |
| Start | `0` | Menunjukkan tipe akrual biaya Start. |
| Prorated | `1` | Menunjukkan tipe akrual biaya Prorated. |
| End | `2` | Menunjukkan tipe akrual biaya End. |
| Invalid | `3` | Menunjukkan tipe akrual biaya Invalid. |

## Catatan

Saat mengekspor ke XML nilai Undefined akan dihilangkan dari XML yang dihasilkan.

## Contoh

Menampilkan cara dan kapan biaya standar dan lembur sumber daya harus dibebankan, atau diakumulasi (metode akrual: Menentukan kapan biaya untuk sebuah sumber daya terjadi dan kapan biaya aktual dibebankan ke proyek. Anda dapat menimbulkan biaya pada awal [Start] atau akhir [End] sebuah tugas atau memprorata mereka [Prorated] selama tugas.), ke biaya sebuah tugas (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// atur tipe akrual biaya
// jika Anda memilih opsi End, biaya tidak diakumulasi sampai pekerjaan yang tersisa menjadi nol.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// bekerja dengan proyek...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


