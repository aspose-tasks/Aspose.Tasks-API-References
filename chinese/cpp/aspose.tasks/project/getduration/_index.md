---
title: "Aspose::Tasks::Project::GetDuration 方法"
linktitle: "GetDuration"
articleTitle: "GetDuration"
second_title: "Aspose.Tasks for C++"
description: "获取具有指定单位数和默认持续时间格式的 Duration 对象，默认持续时间格式在项目的设置 Prj::DurationFormat 中定义。"
type: docs
weight: 1080
url: /zh/cpp/aspose.tasks/project/getduration/
---

## GetDuration (1 of 3) {#getduration_1}

获取具有指定单位数和默认持续时间格式的 Duration 对象，默认持续时间格式在项目的设置 Prj::DurationFormat 中定义。

**Returns:** Duration object.

```cpp
GetDuration(double val)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 值 | 指定的单位数量。 |

---

## GetDuration (2 of 3) {#getduration_2}

获取具有指定数量的 TimeUnitType 单位的 Duration 对象。

**Returns:** Duration object.

```cpp
GetDuration(double val, TimeUnitType timeUnit)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 值 | 指定的单位数量。 |
| timeUnit | 指定的 TimeUnitType 值。 |

---

## GetDuration (3 of 3) {#getduration_3}

获取具有指定 TimeSpan 值和指定 TimeUnitType 值的 Duration 对象。

**Returns:** Duration object.

```cpp
GetDuration(System::TimeSpan timeSpan, TimeUnitType timeUnit)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| timeSpan | 指定的 TimeSpan 值。 |
| timeUnit | 指定的 TimeUnitType 值。 |

