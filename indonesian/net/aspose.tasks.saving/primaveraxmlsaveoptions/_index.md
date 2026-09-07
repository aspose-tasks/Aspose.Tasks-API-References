---
title: "Kelas PrimaveraXmlSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.PrimaveraXmlSaveOptions. Memungkinkan menentukan opsi tambahan saat menyimpan proyek ke format xml Primavera"
type: docs
weight: 2160
url: /id/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Mengizinkan untuk menentukan opsi tambahan saat menyimpan proyek ke format XML Primavera.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | Menginisialisasi instance baru dari kelas `PrimaveraXmlSaveOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menyimpan tugas root atau tidak. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |

## Contoh

Menampilkan cara mengekspor ke file Primavera XML.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Lihat Juga

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


