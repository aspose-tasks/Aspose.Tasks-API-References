---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete 메서드"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "C++용 Aspose.Tasks"
description: "전체 프로젝트에 대해 지정된 날짜까지 모든 작업을 완료된 것으로 업데이트합니다."
type: docs
weight: 2080
url: /ko/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

전체 프로젝트에 대해 지정된 날짜까지 모든 작업을 완료된 것으로 업데이트합니다.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| 매개변수 | 설명 |
| --- | --- |
| completeThrough | 작업을 완료된 상태로 업데이트할 날짜. |
| setZeroOrHundredPercentCompleteOnly | true 로 설정하면 지정된 complete-through 날짜 이전에 종료 날짜가 있는 작업만 100% 완료된 것으로 업데이트합니다. 그렇지 않으면 예정된 시작 날짜와 complete-through 날짜를 기반으로 완료 비율 값을 계산합니다. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

지정된 작업 목록에 대해 지정된 날짜까지 모든 작업을 완료된 상태로 업데이트합니다.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| 매개변수 | 설명 |
| --- | --- |
| completeThrough | 작업을 완료된 상태로 업데이트할 날짜. |
| setZeroOrHundredPercentCompleteOnly | true 로 설정하면 지정된 complete-through 날짜 이전에 종료 날짜가 있는 작업만 100% 완료된 것으로 업데이트합니다. 그렇지 않으면 예정된 시작 날짜와 complete-through 날짜를 기반으로 완료 비율 값을 계산합니다. |
| taskCollection | 작업을 업데이트할 작업들의 List< Task >. |

