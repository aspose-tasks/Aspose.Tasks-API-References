---
title: TimephasedData.CreateUnitTimephased
second_title: Справочник по Aspose.Tasks для .NET API
description: TimephasedData метод. Создает и инициализирует новый экземплярTimephasedData класс для повременных данных назначения материального ресурса в единицах времени.
type: docs
weight: 30
url: /ru/net/aspose.tasks/timephaseddata/createunittimephased/
---
## TimephasedData.CreateUnitTimephased method

Создает и инициализирует новый экземпляр[`TimephasedData`](../) класс для повременных данных назначения материального ресурса в единицах времени.

```csharp
public static TimephasedData CreateUnitTimephased(int uid, DateTime start, DateTime finish, 
    double units, TimephasedDataType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | Int32 | UID задачи. |
| start | DateTime | Дата-время начала. |
| finish | DateTime | Закончить дату-время. |
| units | Double | Количество единиц. |
| type | TimephasedDataType | Поэтапный тип данных. |

### Возвращаемое значение

Экземпляр[`TimephasedData`](../) класс для поэтапных данных на основе затрат.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Если было указано отрицательное количество единиц. |

### Смотрите также

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* пространство имен [Aspose.Tasks](../../timephaseddata/)
* сборка [Aspose.Tasks](../../../)


