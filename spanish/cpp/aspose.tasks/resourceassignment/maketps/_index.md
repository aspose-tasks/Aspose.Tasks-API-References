---
title: "Aspose::Tasks::ResourceAssignment::MakeTPs método"
linktitle: "MakeTPs"
articleTitle: "MakeTPs"
second_title: "Aspose.Tasks for C++"
description: "Genera una lista de datos por fases de tiempo."
type: docs
weight: 740
url: /es/cpp/aspose.tasks/resourceassignment/maketps/
---

## MakeTPs {#maketps}

Genera una lista de datos por fases de tiempo.

**Returns:** A maximum date from list or start date if list is empty.

```cpp
MakeTPs(System::DateTime start, System::TimeSpan time, const System::SharedPtr< Calendar > & calendar, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Aspose::Tasks::TimephasedData >>> & list, bool isWorking, int32_t type)
```

| Parámetro | Descripción |
| --- | --- |
| inicio | La fecha de inicio especificada. |
| tiempo | El tiempo de trabajo especificado. |
| calendario | El calendario de trabajo especificado. |
| lista | La lista de datos con fase temporal. |
| isWorking | La bandera especificada que indica si los datos con fase temporal están activos o no. |
| type | El tipo de datos con fase temporal especificado. |

