---
title: "Aspose::Tasks::Project::GetPageCount 方法"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks for C++"
description: "返回使用默认 Timescale（天）渲染的项目的页数。"
type: docs
weight: 1090
url: /zh/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

返回使用默认 Timescale（天）渲染的项目的页数。

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

返回使用给定 SaveOptions 渲染项目的页数。

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| saveOptions | 用于获取页数的保存选项。 |

---

## GetPageCount (3 of 7) {#getpagecount_3}

返回使用给定 Timescale 和 PageSize 渲染的项目的页数。

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| pageSize | 获取页数的大小。 |
| scale | 获取页数的比例。 |

---

## GetPageCount (4 of 7) {#getpagecount_4}

返回使用给定 Timescale、PresentationFormat 和日期范围渲染的项目的页数。

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| pageSize | 获取页数的大小。 |
| scale | 获取页数的比例。 |
| startDate | 获取页数的开始日期。 |
| endDate | 获取页数的结束日期。 |

---

## GetPageCount (5 of 7) {#getpagecount_5}

返回使用默认 Timescale（Days）和给定 PresentationFormat 渲染的项目的页数。

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 格式 | 获取页数的格式。 |

---

## GetPageCount (6 of 7) {#getpagecount_6}

返回使用给定 Timescale 和 PresentationFormat 渲染的项目的页数。

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 格式 | 获取页数的格式。 |
| scale | 获取页数的比例。 |

---

## GetPageCount (7 of 7) {#getpagecount_7}

返回使用给定 Timescale 渲染的项目的页数。

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| scale | 获取页数的比例。 |

