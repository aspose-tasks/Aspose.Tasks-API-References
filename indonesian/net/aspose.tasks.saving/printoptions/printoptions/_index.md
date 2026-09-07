---
title: "PrintOptions.PrintOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "PrintOptions konstruktor. Menginisialisasi sebuah instance baru dari kelas PrintOptions yang dapat digunakan untuk mengatur berbagai opsi mencetak proyek"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

Menginisialisasi sebuah instance baru dari kelas [`PrintOptions`](../) yang dapat digunakan untuk mengatur berbagai opsi mencetak proyek.

```csharp
public PrintOptions()
```

## Contoh

Menampilkan cara menggunakan opsi pencetakan.

```csharp
try
{
    var project = new Project(DataDir + "Project2.mpp");
    var options = new PrintOptions
    {
        Timescale = Timescale.ThirdsOfMonths
    };
    if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
    {
        project.Print(options);
    }
}
catch (NoPrinterInstalledException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


