---
title: "Prj.FyStartDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Месяц начала финансового года"
type: docs
weight: 350
url: /ru/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

Месяц начала финансового года.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
```

## Примеры

Показывает, как записывать свойства финансового года.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Установить свойства финансового года
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Отобразить свойства финансового года
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


