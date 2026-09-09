---
title: "Prj.FiscalYearStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Mali yıl numaralandırmasının kullanılıp kullanılmayacağını belirler"
type: docs
weight: 340
url: /tr/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

Mali yıl numaralandırmasının kullanılıp kullanılmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
```

## Örnekler

Mali yıl özelliklerinin nasıl yazılacağını gösterir.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Mali yıl özelliklerini ayarla
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Mali yıl özelliklerini göster
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


