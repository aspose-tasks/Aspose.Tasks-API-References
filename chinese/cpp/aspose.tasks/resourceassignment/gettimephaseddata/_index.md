---
title: "Aspose::Tasks::ResourceAssignment::GetTimephasedData 方法"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks for C++"
description: "返回 TimephasedDataCollection 对象，其中包含在给定的 TimephasedDataType::AssignmentWork 的起止日期范围内的 TimephasedData 类实例。"
type: docs
weight: 720
url: /zh/cpp/aspose.tasks/resourceassignment/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

返回 TimephasedDataCollection 对象，其中包含在给定的 TimephasedDataType::AssignmentWork 的起止日期范围内的 TimephasedData 类实例。

**Returns:** returns a list containing instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 开始 | 时间分段数据的开始日期。 |
| end | 时间分段数据的结束日期。 |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

返回 TimephasedDataCollection 类的实例，其中包含在指定 TimephasedDataType 的给定开始和结束日期范围内的 TimephasedData 类实例。

**Returns:** returns a list which contains instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 开始 | 时间分段数据的开始日期。 |
| end | 时间分段数据的结束日期。 |
| timephasedType | 时间分段数据的类型（ Aspose::Tasks::TimephasedDataType ）。 |

