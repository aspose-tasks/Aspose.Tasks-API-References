---
title: "Aspose::Tasks::Task::GetTimephasedData metodu"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "C++ için Aspose.Tasks"
description: "Belirtilen başlangıç ve bitiş tarihleri arasındaki TimephasedData değerlerine sahip bir TimephasedDataCollection nesnesi döndürür."
type: docs
weight: 1360
url: /tr/cpp/aspose.tasks/task/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

Belirtilen başlangıç ve bitiş tarihleri arasındaki TimephasedData değerlerine sahip bir TimephasedDataCollection nesnesi döndürür.

**Returns:** List of Aspose::Tasks::TimephasedData to be filled in.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| Parametre | Açıklama |
| --- | --- |
| başlangıç | Zaman aşamalı veri için başlangıç tarihi. |
| end | Zaman aşamalı veri için bitiş tarihi. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

Belirtilen zaman-fazlı veri türünün verilen başlangıç ve bitiş tarihleri içinde TimephasedData değerleri içeren TimephasedDataCollection nesnesini döndürür.

**Returns:** A TimephasedDataCollection object with TimephasedData values within given start and end dates of specified timephased data type.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| Parametre | Açıklama |
| --- | --- |
| başlangıç | Zaman aşamalı veri için başlangıç tarihi. |
| end | Zaman aşamalı veri için bitiş tarihi. |
| timephasedType | Zaman aşamalı veri türü ( Aspose::Tasks::TimephasedDataType ). |

