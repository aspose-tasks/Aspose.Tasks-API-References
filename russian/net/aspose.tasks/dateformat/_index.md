---
title: "Перечисление DateFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.DateFormat. Указывает формат даты"
type: docs
weight: 430
url: /ru/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Указывает формат даты.

```csharp
public enum DateFormat
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | Пример: 09/30/02 13:00 PM |
| DateMmDdYy | `1` | Пример: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | Пример: September 30, 2002 13:00 PM |
| DateMmmmDdYyyy | `3` | Пример: September 30, 2002 |
| DateMmmDdHhMmAM | `4` | Пример: Sep 30 13:00 PM |
| DateMmmDdYyy | `5` | Пример: Sep 30, '02 |
| DateMmmmDd | `6` | Пример: September 30 |
| DateMmmDd | `7` | Пример: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | Пример: Tue 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | Пример: Tue 9/30/02 |
| DateDddMmmDdYyy | `10` | Пример: Tue Sep 30, '02 |
| DateDddHhMmAM | `11` | Пример: Tue 13:00 PM |
| DateMmDd | `12` | Пример: 9/30 |
| DateDd | `13` | Пример: 30 |
| DateHhMmAm | `14` | Пример: 13:00 PM |
| DateDddMmmDd | `15` | Пример: Tue Sep 30 |
| DateDddMmDd | `16` | Пример: Tue 9/30 |
| DateDddDd | `17` | Пример: Tue 30 |
| DateWwwDd | `18` | Пример: W41/2 |
| DateWwwDdYyHhMmAm | `19` | Пример: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | Пример: 9/30/2002 |
| Custom | `21` | Значения DateTime форматируются с помощью строкового формата, который установлен в свойстве [`CustomDateFormat`](../prj/customdateformat/) проекта. |
| DateDdMmYyyy | `256` | Пример: 19/07/2016 |
| Default | `255` | Пример: Формат даты по умолчанию. |

## Примеры

Показывает, как настроить формат даты всех дат в проекте для экспорта.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// По умолчанию project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) настройте DateFormat (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// Экспорт в формат даты 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


