---
title: "Aspose::Tasks::TaskLinkCollection::Add method"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks for C++"
description: "Returns an instance of Finish-Start TaskLink which has been added to the TaskLinkCollection object."
type: docs
weight: 10
url: /cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

Returns an instance of Finish-Start TaskLink which has been added to the TaskLinkCollection object.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| Parameter | Description |
| --- | --- |
| pred | Predecessor task. |
| succ | Successor task. |

---

## Add (2 of 4) {#add_2}

Returns an instance of TaskLink which has been added to the TaskLinkCollection object.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| Parameter | Description |
| --- | --- |
| pred | Predecessor task. |
| succ | Successor task. |
| linkType | Link type TaskLinkType |

---

## Add (3 of 4) {#add_3}

Returns an instance of TaskLink which has been added to the TaskLinkCollection object.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| Parameter | Description |
| --- | --- |
| pred | Predecessor task. |
| succ | Successor task. |
| linkType | Link type TaskLinkType |
| lag | Link lag Duration . |

---

## Add (4 of 4) {#add_4}

This is the stub implementation of ICollection's Add method, that only throws NotSupportedException

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| Parameter | Description |
| --- | --- |
| item | The item to add. |

