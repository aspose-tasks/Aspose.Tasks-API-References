---
title: "Prj.FyStartDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Bulan ketika tahun fiskal dimulai"
type: docs
weight: 350
url: /id/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

Bulan ketika tahun fiskal dimulai.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
```

## Contoh

Menampilkan cara menulis properti tahun fiskal.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Atur properti tahun fiskal
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Tampilkan properti tahun fiskal
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


