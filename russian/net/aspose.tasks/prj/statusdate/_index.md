---
title: "Prj.StatusDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Дата статуса для отображения прогресса или расчёта сумм заработанной стоимости. Дата статуса совпадает с текущей датой, сегодняшним днём, если не указана другая дата статуса"
type: docs
weight: 690
url: /ru/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

Дата статуса для отображения прогресса или расчёта сумм заработанной стоимости. Дата статуса совпадает с текущей датой (датой сегодня), если не указана другая дата статуса.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Примеры

Показывает, как читать/записывать свойство Prj.StatusDate.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


