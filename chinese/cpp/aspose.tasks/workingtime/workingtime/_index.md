---
title: "Aspose::Tasks::WorkingTime::WorkingTime 构造函数"
linktitle: "WorkingTime"
articleTitle: "WorkingTime"
second_title: "Aspose.Tasks for C++"
description: "使用指定的开始和结束时间初始化 WorkingTime 类的新实例。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/workingtime/workingtime/
---

## WorkingTime (1 of 3) {#workingtime_1}

使用指定的开始和结束时间初始化 WorkingTime 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::DateTime fromTime, System::DateTime toTime)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| fromTime | 间隔开始时间 |
| toTime | 间隔结束时间 |

---

## WorkingTime (2 of 3) {#workingtime_2}

使用具有指定开始和结束时间的间隔项初始化 WorkingTime 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(System::TimeSpan fromTime, System::TimeSpan toTime)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| fromTime | 间隔的开始时间由 TimeSpan 结构表示。 |
| toTime | 间隔的结束时间由 TimeSpan 结构表示。 |

---

## WorkingTime (3 of 3) {#workingtime_3}

使用具有指定开始和结束时间的间隔项初始化 WorkingTime 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
WorkingTime(int32_t fromHours, int32_t toHours)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| fromHours | 间隔的开始时间以整数小时表示（0-24）。 |
| toHours | 间隔的结束时间以整数小时表示（0-24）。 |

