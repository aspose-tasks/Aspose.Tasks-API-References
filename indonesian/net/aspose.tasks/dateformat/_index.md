---
title: "Enum DateFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.DateFormat. Menentukan format tanggal."
type: docs
weight: 430
url: /id/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Menentukan format tanggal.

```csharp
public enum DateFormat
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | Contoh: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | Contoh: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | Contoh: September 30, 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | Contoh: September 30, 2002 |
| DateMmmDdHhMmAM | `4` | Contoh: Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | Contoh: Sep 30, '02 |
| DateMmmmDd | `6` | Contoh: September 30 |
| DateMmmDd | `7` | Contoh: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | Contoh: Sel 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | Contoh: Sel 9/30/02 |
| DateDddMmmDdYyy | `10` | Contoh: Sel Sep 30, '02 |
| DateDddHhMmAM | `11` | Contoh: Sel 13:00 PM |
| DateMmDd | `12` | Contoh: 9/30 |
| DateDd | `13` | Contoh: 30 |
| DateHhMmAm | `14` | Contoh: 13:00 PM |
| DateDddMmmDd | `15` | Contoh: Sel Sep 30 |
| DateDddMmDd | `16` | Contoh: Sel 9/30 |
| DateDddDd | `17` | Contoh: Sel 30 |
| DateWwwDd | `18` | Contoh: W41/2 |
| DateWwwDdYyHhMmAm | `19` | Contoh: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | Contoh: 9/30/2002 |
| Custom | `21` | Nilai DateTime diformat menggunakan string format yang ditetapkan pada properti [`CustomDateFormat`](../prj/customdateformat/) proyek. |
| DateDdMmYyyy | `256` | Contoh: 19/07/2016 |
| Default | `255` | Contoh: Format tanggal default. |

## Contoh

Menampilkan cara menyesuaikan format tanggal semua tanggal dalam proyek yang akan diekspor.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// Secara default project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) sesuaikan DateFormat (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// Ekspor ke format tanggal 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


