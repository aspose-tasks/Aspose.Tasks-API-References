---
title: "Aspose::Tasks::TaskLinkCollection::Add 方法"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks for C++"
description: "返回已添加到 TaskLinkCollection 对象的结束-开始 TaskLink 实例。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

返回已添加到 TaskLinkCollection 对象的结束-开始 TaskLink 实例。

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| pred | 前置任务。 |
| succ | 后继任务。 |

---

## Add (2 of 4) {#add_2}

返回已添加到 TaskLinkCollection 对象的 TaskLink 实例。

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| pred | 前置任务。 |
| succ | 后继任务。 |
| linkType | 链接类型 TaskLinkType |

---

## Add (3 of 4) {#add_3}

返回已添加到 TaskLinkCollection 对象的 TaskLink 实例。

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| pred | 前置任务。 |
| succ | 后继任务。 |
| linkType | 链接类型 TaskLinkType |
| lag | 链接延迟持续时间。 |

---

## Add (4 of 4) {#add_4}

这是 ICollection 的 Add 方法的存根实现，只会抛出 NotSupportedException。

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| 参数 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| 项目 | 要添加的项。 |

