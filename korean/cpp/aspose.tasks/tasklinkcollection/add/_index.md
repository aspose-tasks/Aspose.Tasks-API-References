---
title: "Aspose::Tasks::TaskLinkCollection::Add 메서드"
linktitle: "추가"
articleTitle: "추가"
second_title: "C++용 Aspose.Tasks"
description: "TaskLinkCollection 객체에 추가된 Finish-Start TaskLink 인스턴스를 반환합니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/tasklinkcollection/add/
---

## Add (1 of 4) {#add_1}

TaskLinkCollection 객체에 추가된 Finish-Start TaskLink 인스턴스를 반환합니다.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ)
```

| 매개변수 | 설명 |
| --- | --- |
| pred | 선행 작업. |
| succ | 후속 작업. |

---

## Add (2 of 4) {#add_2}

TaskLinkCollection 객체에 추가된 TaskLink 인스턴스를 반환합니다.

**Returns:** a task link instance which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType)
```

| 매개변수 | 설명 |
| --- | --- |
| pred | 선행 작업. |
| succ | 후속 작업. |
| linkType | 링크 유형 TaskLinkType |

---

## Add (3 of 4) {#add_3}

TaskLinkCollection 객체에 추가된 TaskLink 인스턴스를 반환합니다.

**Returns:** a task link which has been added to this object.

```cpp
Add(const System::SharedPtr< Task > & pred, const System::SharedPtr< Task > & succ, TaskLinkType linkType, Duration lag)
```

| 매개변수 | 설명 |
| --- | --- |
| pred | 선행 작업. |
| succ | 후속 작업. |
| linkType | 링크 유형 TaskLinkType |
| lag | 링크 지연 기간. |

---

## Add (4 of 4) {#add_4}

이것은 ICollection의 Add 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다.

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< TaskLink > & item)
```

| 매개변수 | 설명 |
| --- | --- |
| 항목 | 추가할 항목. |

