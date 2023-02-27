---
title: TimephasedData.CreateWorkTimephased
second_title: Справочник по Aspose.Tasks для .NET API
description: TimephasedData метод. Создает и инициализирует новый экземплярTimephasedData класс для поэтапных данных на основе работы.
type: docs
weight: 40
url: /ru/net/aspose.tasks/timephaseddata/createworktimephased/
---
## TimephasedData.CreateWorkTimephased method

Создает и инициализирует новый экземпляр[`TimephasedData`](../) класс для поэтапных данных на основе работы.

```csharp
public static TimephasedData CreateWorkTimephased(int uid, DateTime start, DateTime finish, 
    TimeSpan value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | Int32 | UID задачи. |
| start | DateTime | дата-время начала. |
| finish | DateTime | Закончить дату-время. |
| value | TimeSpan | Значение временного промежутка. |
| timeUnit | TimeUnitType | Тип единицы времени. |
| type | TimephasedDataType | Поэтапный тип данных. |

### Возвращаемое значение

Экземпляр[`TimephasedData`](../) класс для поэтапных данных на основе работы.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Если было указано отрицательное значение работы. |

### Смотрите также

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* пространство имен [Aspose.Tasks](../../timephaseddata/)
* сборка [Aspose.Tasks](../../../)


