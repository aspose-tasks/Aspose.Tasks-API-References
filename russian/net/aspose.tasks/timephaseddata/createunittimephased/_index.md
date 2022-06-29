---
title: CreateUnitTimephased
second_title: Справочник по Aspose.Tasks для .NET API
description: Создает и инициализирует новый экземпляр классаTimephasedDataaspose.tasks/timephaseddataдля повременных данных назначения материальный ресурс.
type: docs
weight: 30
url: /ru/net/aspose.tasks/timephaseddata/createunittimephased/
---
## TimephasedData.CreateUnitTimephased method

Создает и инициализирует новый экземпляр класса[`TimephasedData`](../../timephaseddata)для повременных данных назначения материальный ресурс.

```csharp
public static TimephasedData CreateUnitTimephased(int uid, DateTime start, DateTime finish, 
    double units, TimephasedDataType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | Int32 | UID задачи. |
| start | DateTime | Дата и время начала. |
| finish | DateTime | Дата-время окончания. |
| units | Double | Количество юнитов. |
| type | TimephasedDataType | Поэтапный тип данных. |

### Возвращаемое значение

Экземпляр класса[`TimephasedData`](../../timephaseddata)для поэтапных данных на основе затрат по времени.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Если было указано отрицательное количество единиц. |

### Смотрите также

* enum [TimephasedDataType](../../timephaseddatatype)
* class [TimephasedData](../../timephaseddata)
* пространство имен [Aspose.Tasks](../../timephaseddata)
* сборка [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->