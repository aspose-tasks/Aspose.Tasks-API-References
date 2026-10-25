---
title: "Aspose::Tasks::Task::GetTimephasedData metodo"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks per C++"
description: "Restituisce un oggetto TimephasedDataCollection con i valori TimephasedData compresi tra le date di inizio e fine specificate."
type: docs
weight: 1360
url: /it/cpp/aspose.tasks/task/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

Restituisce un oggetto TimephasedDataCollection con i valori TimephasedData compresi tra le date di inizio e fine specificate.

**Returns:** List of Aspose::Tasks::TimephasedData to be filled in.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| Parametro | Descrizione |
| --- | --- |
| avvio | La data di inizio per i dati a intervalli temporali. |
| end | La data di fine per i dati a intervalli temporali. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

Restituisce l'oggetto TimephasedDataCollection con i valori TimephasedData compresi tra le date di inizio e fine fornite per il tipo di dati temporizzati specificato.

**Returns:** A TimephasedDataCollection object with TimephasedData values within given start and end dates of specified timephased data type.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| Parametro | Descrizione |
| --- | --- |
| avvio | La data di inizio per i dati a intervalli temporali. |
| end | La data di fine per i dati a intervalli temporali. |
| timephasedType | Il tipo di dati a intervalli temporali ( Aspose::Tasks::TimephasedDataType ). |

