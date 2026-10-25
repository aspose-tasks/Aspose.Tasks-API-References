---
title: "Aspose::Tasks::Resource::GetTimephasedData метод"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks для C++"
description: "Возвращает TimephasedDataCollection для этого объекта со значениями TimephasedData в указанных начальной и конечной датах."
type: docs
weight: 850
url: /ru/cpp/aspose.tasks/resource/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

Возвращает TimephasedDataCollection для этого объекта со значениями TimephasedData в указанных начальной и конечной датах.

**Returns:** List of Aspose::Tasks::TimephasedData .

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| Параметр | Описание |
| --- | --- |
| начало | Дата начала для фазированных данных. |
| end | Дата окончания для данных с фазированием по времени. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

Возвращает экземпляр класса TimephasedDataCollection для этого объекта со значениями TimephasedData в пределах заданных дат начала и окончания указанного TimephasedDataType.

**Returns:** List of TimephasedData .

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| Параметр | Описание |
| --- | --- |
| начало | Дата начала для фазированных данных. |
| end | Дата окончания для данных с фазированием по времени. |
| timephasedType | Тип данных с фазированием по времени ( Aspose::Tasks::TimephasedDataType ). |

