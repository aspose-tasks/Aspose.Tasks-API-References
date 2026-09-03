---
title: "Aspose::Tasks::Task::GetTimephasedData μέθοδος"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks για C++"
description: "Επιστρέφει ένα αντικείμενο TimephasedDataCollection με τιμές TimephasedData εντός των δοσμένων ημερομηνιών έναρξης και λήξης."
type: docs
weight: 1360
url: /el/cpp/aspose.tasks/task/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

Επιστρέφει ένα αντικείμενο TimephasedDataCollection με τιμές TimephasedData εντός των δοσμένων ημερομηνιών έναρξης και λήξης.

**Returns:** List of Aspose::Tasks::TimephasedData to be filled in.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| έναρξη | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| end | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

Επιστρέφει αντικείμενο TimephasedDataCollection με τιμές TimephasedData εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου τύπου χρονομετρικών δεδομένων.

**Returns:** A TimephasedDataCollection object with TimephasedData values within given start and end dates of specified timephased data type.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| έναρξη | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| end | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |
| timephasedType | Ο τύπος των δεδομένων χρονικής φάσης ( Aspose::Tasks::TimephasedDataType ). |

