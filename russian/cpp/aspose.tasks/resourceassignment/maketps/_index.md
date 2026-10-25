---
title: "Aspose::Tasks::ResourceAssignment::MakeTPs метод"
linktitle: "MakeTPs"
articleTitle: "MakeTPs"
second_title: "Aspose.Tasks для C++"
description: "Генерирует список данных с временной разбивкой."
type: docs
weight: 740
url: /ru/cpp/aspose.tasks/resourceassignment/maketps/
---

## MakeTPs {#maketps}

Генерирует список данных с временной разбивкой.

**Returns:** A maximum date from list or start date if list is empty.

```cpp
MakeTPs(System::DateTime start, System::TimeSpan time, const System::SharedPtr< Calendar > & calendar, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Aspose::Tasks::TimephasedData >>> & list, bool isWorking, int32_t type)
```

| Параметр | Описание |
| --- | --- |
| начало | Указанная дата начала. |
| время | Указанное рабочее время. |
| календарь | Указанный рабочий календарь. |
| список | Список данных с фазированием во времени. |
| isWorking | Указанный флаг, определяющий, является ли данные с фазированием во времени рабочими или нет. |
| type | Указанный тип данных с фазированием во времени. |

