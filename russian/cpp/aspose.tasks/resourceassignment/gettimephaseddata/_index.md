---
title: "Aspose::Tasks::ResourceAssignment::GetTimephasedData метод"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks для C++"
description: "Возвращает объект TimephasedDataCollection с экземплярами класса TimephasedData в пределах заданных дат начала и окончания типа TimephasedDataType::AssignmentWork."
type: docs
weight: 720
url: /ru/cpp/aspose.tasks/resourceassignment/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

Возвращает объект TimephasedDataCollection с экземплярами класса TimephasedData в пределах заданных дат начала и окончания типа TimephasedDataType::AssignmentWork.

**Returns:** returns a list containing instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| Параметр | Описание |
| --- | --- |
| начало | Дата начала для фазированных данных. |
| end | Дата окончания для данных с фазированием по времени. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

Возвращает экземпляр класса TimephasedDataCollection, содержащий экземпляры класса TimephasedData в указанных датах начала и окончания заданного типа TimephasedDataType.

**Returns:** returns a list which contains instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| Параметр | Описание |
| --- | --- |
| начало | Дата начала для фазированных данных. |
| end | Дата окончания для данных с фазированием по времени. |
| timephasedType | Тип данных с фазированием по времени ( Aspose::Tasks::TimephasedDataType ). |

