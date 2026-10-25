---
title: "Aspose::Tasks::ResourceAssignment::MakeTPs 方法"
linktitle: "MakeTPs"
articleTitle: "MakeTPs"
second_title: "Aspose.Tasks for C++"
description: "生成分阶段数据的列表。"
type: docs
weight: 740
url: /zh/cpp/aspose.tasks/resourceassignment/maketps/
---

## MakeTPs {#maketps}

生成分阶段数据的列表。

**Returns:** A maximum date from list or start date if list is empty.

```cpp
MakeTPs(System::DateTime start, System::TimeSpan time, const System::SharedPtr< Calendar > & calendar, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Aspose::Tasks::TimephasedData >>> & list, bool isWorking, int32_t type)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 开始 | 指定的开始日期。 |
| 时间 | 指定的工作时间。 |
| 日历 | 指定的工作日历。 |
| 列表 | 时间分段数据的列表。 |
| isWorking | 指定的标志，用于指示时间分段数据是否为工作状态。 |
| type | 指定的时间分段数据类型。 |

