---
title: TimephasedData.CreateCostTimephased
second_title: Справочник по Aspose.Tasks для .NET API
description: TimephasedData метод. Создает и инициализирует новый экземплярTimephasedData класс для поэтапных данных на основе затрат.
type: docs
weight: 20
url: /ru/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

Создает и инициализирует новый экземпляр[`TimephasedData`](../) класс для поэтапных данных на основе затрат.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | Int32 | UID задачи. |
| start | DateTime | дата-время начала. |
| finish | DateTime | Закончить дату-время. |
| value | Double | Стоимость. |
| timeUnit | TimeUnitType | Тип единицы времени. |
| type | TimephasedDataType | Поэтапный тип данных. |

### Возвращаемое значение

Экземпляр[`TimephasedData`](../) класс для поэтапных данных на основе затрат.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Если было указано отрицательное значение стоимости. |

### Смотрите также

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* пространство имен [Aspose.Tasks](../../timephaseddata/)
* сборка [Aspose.Tasks](../../../)


