---
title: "Aspose::Tasks::Project::Project 构造函数"
linktitle: "项目"
articleTitle: "项目"
second_title: "Aspose.Tasks for C++"
description: "初始化 Project 类的新实例。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/project/project/
---

## Project (1 of 13) {#project_1}

初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project()
```

---

## Project (2 of 13) {#project_2}

从受密码保护的模板（现有的 mpp 或 mpt 文件）初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::String & protectionPassword)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| projectTemplate | 用于创建项目的模板路径。 |
| protectionPassword | 保护密码。 |

---

## Project (3 of 13) {#project_3}

从模板（现有的 mpp 或 mpt 文件）初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| projectTemplate | 用于创建项目的模板路径。 |

---

## Project (4 of 13) {#project_4}

使用 PrimaveraReadOptions 类的指定实例，从 Stream 初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| stream | Project System::IO::Stream 类的 Stream |
| options | 指定的 PrimaveraReadOptions 类实例，允许自定义读取 Primavera 格式（XER 或 XML）。 |

---

## Project (5 of 13) {#project_5}

从模板（现有的 mpp 或 mpt 文件）初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, ParseErrorCallback parseErrorHandler)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| projectTemplate | 用于创建项目的模板路径。 |
| parseErrorHandler | 用于处理 xml 解析错误的指定回调方法。 |

---

## Project (6 of 13) {#project_6}

从流初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| stream | 用于加载模板的流。 |

---

## Project (7 of 13) {#project_7}

从 StreamReader 实例初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::StreamReader > & reader)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| reader | 用于加载模板的流读取器。 |

---

## Project (8 of 13) {#project_8}

使用指定的 PrimaveraReadOptions 类实例，从模板（现有的 MPP 或 MPT 文件）初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< PrimaveraReadOptions > & options)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| projectTemplate | 用于创建项目的模板路径 |
| options | 指定的 PrimaveraReadOptions 类实例。 |

---

## Project (9 of 13) {#project_9}

使用 DbSettings 类实例指定的数据库，初始化 Project 类的新实例以读取数据。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< Connectivity::DbSettings > & settings)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 设置 | 指定的 DbSettings 类实例。 |

---

## Project (10 of 13) {#project_10}

从模板（现有的 mpp 或 mpt 文件）初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, ParseErrorCallback parseErrorHandler)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| stream | 用于加载模板的流。 |
| parseErrorHandler | 用于处理 xml 解析错误的指定回调方法。 |

---

## Project (11 of 13) {#project_11}

从模板（现有的 mpp 或 mpt 文件）初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::String & protectionPassword)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| stream | 用于加载模板的流。 |
| protectionPassword | 保护密码。 |

---

## Project (12 of 13) {#project_12}

使用指定的 LoadOptions 类实例，从模板（现有的 mpp 或 mpt 文件）初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::String & projectTemplate, const System::SharedPtr< LoadOptions > & options)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| projectTemplate | 用于创建项目的模板路径 |
| options | 指定的 LoadOptions 类实例。 |

---

## Project (13 of 13) {#project_13}

使用指定的 LoadOptions 类实例，从流中初始化 Project 类的新实例。

**Returns:** Aspose::Tasks::

```cpp
Project(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< LoadOptions > & options)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| stream | Project System::IO::Stream 类的 Stream |
| options | 指定的 LoadOptions 类实例 |

