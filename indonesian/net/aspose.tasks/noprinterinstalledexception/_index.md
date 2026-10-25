---
title: "Kelas NoPrinterInstalledException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.NoPrinterInstalledException. Mewakili pengecualian yang dilempar ketika tidak ada printer terpasang di OS."
type: docs
weight: 1100
url: /id/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

Mewakili pengecualian yang dilemparkan ketika tidak ada printer terpasang di OS.

```csharp
public class NoPrinterInstalledException : Exception
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


