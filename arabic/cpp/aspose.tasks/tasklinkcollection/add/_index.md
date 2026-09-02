---
title: "طريقة Aspose::Tasks::TaskLinkCollection::Add"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks لـ C++"
description: "يعيد مثيلاً من رابط المهمة من نوع الانتهاء-البداية الذي تم إضافته إلى كائن TaskLinkCollection."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

يعيد مثيلاً من رابط المهمة من نوع الانتهاء-البداية الذي تم إضافته إلى كائن TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| معامل | الوصف |
| --- | --- |
| pred | مهمة سابقة. |
| succ | مهمة لاحقة. |

---

## Add (2 of 4) {#add_2}

يعيد مثيلاً من TaskLink تم إضافته إلى كائن TaskLinkCollection.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| معامل | الوصف |
| --- | --- |
| pred | مهمة سابقة. |
| succ | مهمة لاحقة. |
| linkType | نوع الارتباط TaskLinkType |

---

## Add (3 of 4) {#add_3}

يعيد مثيلاً من TaskLink تم إضافته إلى كائن TaskLinkCollection.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| معامل | الوصف |
| --- | --- |
| pred | مهمة سابقة. |
| succ | مهمة لاحقة. |
| linkType | نوع الارتباط TaskLinkType |
| lag | مدة تأخير الارتباط. |

---

## Add (4 of 4) {#add_4}

هذه هي تنفيذية تجريبية لطريقة Add في ICollection، التي تُطلق فقط استثناء NotSupportedException.

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| معامل | الوصف |
| --- | --- |
| العنصر | العنصر المراد إضافته. |

