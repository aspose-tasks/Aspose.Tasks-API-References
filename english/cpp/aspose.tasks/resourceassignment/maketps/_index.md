---
title: "Aspose::Tasks::ResourceAssignment::MakeTPs method"
linktitle: "MakeTPs"
articleTitle: "MakeTPs"
second_title: "Aspose.Tasks for C++"
description: "Generates a list of time phased data."
type: docs
weight: 740
url: /cpp/aspose.tasks/resourceassignment/maketps/
---

## MakeTPs {#maketps}

Generates a list of time phased data.

**Returns:** A maximum date from list or start date if list is empty.

```cpp
MakeTPs(System::DateTime start, System::TimeSpan time, const System::SharedPtr< Calendar > & calendar, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Aspose::Tasks::TimephasedData >>> & list, bool isWorking, int32_t type)
```

| Parameter | Description |
| --- | --- |
| start | The specified start date. |
| time | The specified working time. |
| calendar | The specified working calendar. |
| list | The list of time phased data. |
| isWorking | The specified flag which specifies whether time-phased data is working or not. |
| type | The specified time-phased data type. |

