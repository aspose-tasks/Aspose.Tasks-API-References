---
title: "Enum DateFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.DateFormat enum. Tarih biçimini belirtir."
type: docs
weight: 430
url: /tr/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Tarih biçimini belirtir.

```csharp
public enum DateFormat
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | Örnek: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | Örnek: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | Örnek: September 30, 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | Örnek: September 30, 2002 |
| DateMmmDdHhMmAM | `4` | Örnek: Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | Örnek: Eyl 30, '02 |
| DateMmmmDd | `6` | Örnek: Eylül 30 |
| DateMmmDd | `7` | Örnek: Eyl 30 |
| DateDddMmDdYyHhMmAM | `8` | Örnek: Sal 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | Örnek: Sal 9/30/02 |
| DateDddMmmDdYyy | `10` | Örnek: Sal Eyl 30, '02 |
| DateDddHhMmAM | `11` | Örnek: Sal 13:00 PM |
| DateMmDd | `12` | Örnek: 9/30 |
| DateDd | `13` | Örnek: 30 |
| DateHhMmAm | `14` | Örnek: 13:00 PM |
| DateDddMmmDd | `15` | Örnek: Sal Eyl 30 |
| DateDddMmDd | `16` | Örnek: Sal 9/30 |
| DateDddDd | `17` | Örnek: Sal 30 |
| DateWwwDd | `18` | Örnek: W41/2 |
| DateWwwDdYyHhMmAm | `19` | Örnek: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | Örnek: 9/30/2002 |
| Custom | `21` | DateTime değerleri, projenin [`CustomDateFormat`](../prj/customdateformat/) özelliğine ayarlanan format dizesi kullanılarak biçimlendirilir. |
| DateDdMmYyyy | `256` | Örnek: 19/07/2016 |
| Default | `255` | Örnek: Varsayılan tarih formatı. |

## Örnekler

Projede dışa aktarılacak tüm tarihlerin tarih formatını nasıl özelleştireceğinizi gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// Varsayılan olarak project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Pzt 09/22/14) DateFormat'i özelleştirin (Eylül 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// 19/07/2016 tarih formatına dışa aktar
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


