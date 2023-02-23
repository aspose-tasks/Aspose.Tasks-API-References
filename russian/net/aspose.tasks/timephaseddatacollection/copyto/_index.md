---
title: TimephasedDataCollection.CopyTo
second_title: Справочник по Aspose.Tasks для .NET API
description: TimephasedDataCollection метод. Копирует элементыTimephasedDataCollection дляArray  начиная с определенногоArray индекс.
type: docs
weight: 90
url: /ru/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

Копирует элементы[`TimephasedDataCollection`](../) дляArray , начиная с определенногоArray индекс.

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| array | TimephasedData[] | одномерныйArray это место назначения элементов, скопированных из[`TimephasedDataCollection`](../) . Array должны иметь индексацию с отсчетом от нуля. |
| arrayIndex | Int32 | Индекс с отсчетом от нуля в*array* при котором начинается копирование. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | *array* нулевой. |
| ArgumentOutOfRangeException | *arrayIndex* меньше 0. |
| ArgumentException | Количество элементов в исходнике[`TimephasedDataCollection`](../) больше, чем доступное пространство от*arrayIndex* до конца пункта назначения*array* . |

### Смотрите также

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* пространство имен [Aspose.Tasks](../../timephaseddatacollection/)
* сборка [Aspose.Tasks](../../../)


