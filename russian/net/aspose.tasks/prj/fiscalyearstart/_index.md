---
title: "Prj.FiscalYearStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, используется ли нумерация финансового года"
type: docs
weight: 340
url: /ru/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

Определяет, используется ли нумерация финансового года.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


