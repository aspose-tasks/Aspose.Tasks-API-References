---
title: "Aspose::Tasks::ResourceAssignment::GetTimephasedData metodo"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks per C++"
description: "Restituisce l'oggetto TimephasedDataCollection con le istanze della classe TimephasedData entro le date di inizio e fine specificate per TimephasedDataType::AssignmentWork."
type: docs
weight: 720
url: /it/cpp/aspose.tasks/resourceassignment/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

Restituisce l'oggetto TimephasedDataCollection con le istanze della classe TimephasedData entro le date di inizio e fine specificate per TimephasedDataType::AssignmentWork.

**Returns:** returns a list containing instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| Parametro | Descrizione |
| --- | --- |
| avvio | La data di inizio per i dati a intervalli temporali. |
| end | La data di fine per i dati a intervalli temporali. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

Restituisce l'istanza della classe TimephasedDataCollection contenente istanze della classe TimephasedData entro le date di inizio e fine specificate per il tipo TimephasedDataType.

**Returns:** returns a list which contains instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| Parametro | Descrizione |
| --- | --- |
| avvio | La data di inizio per i dati a intervalli temporali. |
| end | La data di fine per i dati a intervalli temporali. |
| timephasedType | Il tipo di dati a intervalli temporali ( Aspose::Tasks::TimephasedDataType ). |

