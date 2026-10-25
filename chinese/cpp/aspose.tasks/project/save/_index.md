---
title: "Aspose::Tasks::Project::Save 方法"
linktitle: "Save"
articleTitle: "Save"
second_title: "Aspose.Tasks for C++"
description: "使用指定的保存选项将项目保存到流中。"
type: docs
weight: 1190
url: /zh/cpp/aspose.tasks/project/save/
---

## Save (1 of 5) {#save_1}

使用指定的保存选项将项目保存到流中。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| stream | 流。 |
| options | 保存选项。 |

---

## Save (2 of 5) {#save_2}

将项目数据保存到流中。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::SharedPtr< System::IO::Stream > & stream, Saving::SaveFileFormat format)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| stream | 流。 |
| 格式 | 指定的保存文件格式。SaveFileFormat |

---

## Save (3 of 5) {#save_3}

将项目数据以 mpp 格式保存到文件中。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 文件名 | 文件名。 |

---

## Save (4 of 5) {#save_4}

使用指定的保存选项将文档保存到文件。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, const System::SharedPtr< Saving::SimpleSaveOptions > & options)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 文件名 | 文件名。 |
| options | 保存选项。 |

---

## Save (5 of 5) {#save_5}

将项目数据保存到文件。

**Returns:** void Aspose::Tasks::

```cpp
Save(const System::String & filename, Saving::SaveFileFormat format)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 文件名 | 文件名。 |
| 格式 | 保存文件格式。 |

