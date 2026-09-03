---
title: "Aspose::Tasks::TaskCollection::Add 메서드"
linktitle: "추가"
articleTitle: "추가"
second_title: "C++용 Aspose.Tasks"
description: "마지막 작업과 동일한 개요 수준에서 프로젝트 작업 컬렉션에 새 작업을 추가합니다."
type: docs
weight: 10
url: /ko/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

마지막 작업과 동일한 개요 수준에서 프로젝트 작업 컬렉션에 새 작업을 추가합니다.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

지정된 ID를 가진 작업 앞에 새 작업을 삽입하고 동일한 개요 수준에 배치합니다.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| 매개변수 | 설명 |
| --- | --- |
| 매개변수 | 반복 작업 생성을 위한 지정된 매개변수. |

---

## Add (3 of 5) {#add_3}

지정된 작업을 TaskCollection 클래스의 인스턴스에 추가합니다. ParentProject.CalculationMode가 None인 경우 사용자는 이 메서드 사용 후 Project.Recalculate()를 호출해야 합니다(이 메서드는 모든 프로젝트 작업(시작/종료 날짜, 조기/지연 날짜 설정)을 다시 일정화하고 여유시간, 작업 및 비용 필드, ID 및 개요 수준과 같은 종속 필드를 계산합니다). ParentProject.CalculationMode가 Manual인 경우 메서드는 작업 ID, 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우 메서드는 모든 프로젝트 작업을 자동으로 다시 일정화합니다(시작/종료 날짜, 조기/지연 날짜 설정, 여유시간, 작업 및 비용 필드 계산, ID 및 개요 수준을 다시 계산).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| 매개변수 | 설명 |
| --- | --- |
| 항목 | 이 작업 컬렉션에 추가되어야 하는 지정된 작업입니다. |

---

## Add (4 of 5) {#add_4}

새 작업을 하위 작업 컬렉션에 추가합니다.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| 매개변수 | 설명 |
| --- | --- |
| taskName | 지정된 작업 이름입니다. |

---

## Add (5 of 5) {#add_5}

새 반복 작업을 하위 작업 컬렉션에 추가합니다.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| 매개변수 | 설명 |
| --- | --- |
| taskName | 지정된 작업 이름입니다. |
| beforeTaskId | 새 작업이 삽입될 작업 앞에 있는 지정된 작업 ID입니다. |

