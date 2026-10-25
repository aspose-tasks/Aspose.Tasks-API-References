---
title: "Kelas PrimaveraReadOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.PrimaveraReadOptions. Memungkinkan menentukan opsi tambahan saat membaca file Primavera Xml atau Primavera Xer."
type: docs
weight: 1370
url: /id/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Memungkinkan menentukan opsi tambahan saat membaca file Primavera Xml atau Primavera Xer.

```csharp
public class PrimaveraReadOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Menginisialisasi instance baru dari kelas `PrimaveraReadOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Mendapatkan atau mengatur flag yang menentukan apakah pengidentifikasi unik asli entitas harus dipertahankan. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Mendapatkan atau mengatur UID proyek yang akan dibaca dari file yang berisi beberapa proyek. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Mendapatkan atau mengatur flag yang menentukan apakah proyek baseline harus dimuat. Nilai default adalah true. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | Menentukan perilaku yang digunakan untuk memproses tugas dengan kendala yang tidak terdefinisi yang dibaca dari format XER. |

## Contoh

Menampilkan cara membaca proyek dari file Primavera XML atau Primavera XER yang berisi beberapa proyek.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Mengembalikan proyek dengan UID khusus
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


