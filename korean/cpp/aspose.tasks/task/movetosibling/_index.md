---
title: "Aspose::Tasks::Task::MoveToSibling 메서드"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "C++용 Aspose.Tasks"
description: "현재 작업을 동일한 개요 수준에서 지정된 작업 앞에 이동합니다."
type: docs
weight: 1370
url: /ko/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

현재 작업을 동일한 Outline Level에서 지정된 작업 앞에 이동합니다. ParentProject.CalculationMode가 None인 경우, 이 메서드 사용 후에 Project.Recalculate()를 호출해야 합니다(이렇게 하면 모든 프로젝트 작업(시작/완료 날짜, 조기/지연 날짜 설정)이 재조정되고, 슬랙, 작업 및 비용 필드, Outline Level과 같은 종속 필드가 계산됩니다). ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 ID, Outline Level 및 Outline 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 재조정합니다(시작/완료 날짜, 조기/지연 날짜 설정, 슬랙, 작업 및 비용 필드 계산, ID와 Outline Level 재계산).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| 매개변수 | 설명 |
| --- | --- |
| beforeTask | 현재 작업이 삽입될 작업 앞에 있는 작업. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

현재 작업을 동일한 개요 수준에서 지정된 Id를 가진 작업 앞에 이동합니다. ParentProject.CalculationMode가 None인 경우, 사용자는 이 메서드 사용 후 Project.Recalculate()를 호출해야 합니다(이 메서드는 모든 프로젝트 작업(시작/완료 날짜, 조기/지연 날짜 설정)을 다시 일정하고, 여유시간, 작업 및 비용 필드, 개요 수준과 같은 종속 필드를 계산합니다). ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 Id, 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 다시 일정합니다(시작/완료 날짜, 조기/지연 날짜 설정, 여유시간, 작업 및 비용 필드 계산, Id와 개요 수준을 다시 계산).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| 매개변수 | 설명 |
| --- | --- |
| beforeTaskId | 현재 작업이 삽입될 작업 앞에 있는 작업의 Id ( Tsk::Id ). |

