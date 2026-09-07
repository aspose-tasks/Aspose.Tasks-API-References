---
title: "Prj.FiscalYearStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah penomoran tahun fiskal digunakan"
type: docs
weight: 340
url: /id/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

Menentukan apakah penomoran tahun fiskal digunakan.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


