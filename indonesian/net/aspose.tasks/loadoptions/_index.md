---
title: "Kelas LoadOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.LoadOptions. Memungkinkan untuk menentukan parameter pemuatan tambahan saat memuat proyek dari file atau aliran"
type: docs
weight: 990
url: /id/net/aspose.tasks/loadoptions/
---
## LoadOptions class

Memungkinkan untuk menentukan parameter pemuatan tambahan saat memuat proyek dari file atau aliran.

```csharp
public class LoadOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [LoadOptions](loadoptions/)() | Menginisialisasi instance baru dari kelas `LoadOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Mendapatkan atau mengatur token yang dapat digunakan untuk membatalkan operasi pemuatan proyek. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | Mendapatkan atau mengatur encoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML. Encoding default adalah UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | Mendapatkan atau mengatur metode callback untuk menangani kesalahan parsing xml. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Mendapatkan atau mengatur kata sandi perlindungan. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | Mendapatkan atau mengatur instance tertentu dari kelas [`PrimaveraReadOptions`](../primaverareadoptions/) yang dapat digunakan untuk menyesuaikan perilaku pemuatan format Primavera (Primavera P6 XER atau Primavera P6 Xml). |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | Mendapatkan atau mengatur callback yang akan dipanggil selama operasi pemuatan proyek. Saat ini didukung untuk format MPP dan XER. |

## Contoh

Menampilkan cara memuat proyek yang dilindungi kata sandi menggunakan instance &lt;see cref="Aspose.Tasks.LoadOptions"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


