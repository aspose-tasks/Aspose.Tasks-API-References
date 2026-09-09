---
title: "Prj.FyStartDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Mali yılın başladığı ay"
type: docs
weight: 350
url: /tr/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

Mali yılın başladığı ay.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
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
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


