---
title: TimephasedDataCollection.SelectBetweenStartAndFinish
second_title: Справочник по Aspose.Tasks для .NET API
description: TimephasedDataCollection метод. Выбирает все временные фазы междуstartTime иfinishTime . В среднем имеет сложность Olog n.
type: docs
weight: 120
url: /ru/net/aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/
---
## TimephasedDataCollection.SelectBetweenStartAndFinish method

Выбирает все временные фазы между*startTime* и*finishTime* . В среднем имеет сложность O(log n).

```csharp
public IList<TimephasedData> SelectBetweenStartAndFinish(TimephasedDataType timephasedDataType, 
    DateTime startTime, DateTime finishTime)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| timephasedDataType | TimephasedDataType | Тип временных фаз для выбора. |
| startTime | DateTime | Начало интервала. |
| finishTime | DateTime | Окончание интервала. |

### Возвращаемое значение

Возвращает новый экземпляр списка[`TimephasedDataCollection`](../) данные, упорядоченные по свойству Start.

### Смотрите также

* class [TimephasedData](../../timephaseddata/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedDataCollection](../)
* пространство имен [Aspose.Tasks](../../timephaseddatacollection/)
* сборка [Aspose.Tasks](../../../)


