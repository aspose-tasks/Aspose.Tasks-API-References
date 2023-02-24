---
title: TaskCollection
second_title: .NET API 참조용 Aspose.Tasks
description: 컬렉션을 나타냅니다.Task./task/ 객체.
type: docs
weight: 2100
url: /ko/net/aspose.tasks/taskcollection/
---
## TaskCollection class

컬렉션을 나타냅니다.[`Task`](../task/) 객체.

```csharp
public class TaskCollection : IList<Task>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | TaskCollection. 에 포함된 개체 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | 지정된 인덱스에 있는 요소를 반환합니다. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | TaskCollection 개체의 상위 프로젝트를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | 마지막 작업과 동일한 개요 수준에서 프로젝트 작업 컬렉션에 새 작업을 추가합니다. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | 동일한 개요 수준에서 지정된 ID를 가진 작업 앞에 새 작업을 삽입합니다. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | 자식 작업 컬렉션에 새 작업을 추가합니다. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | 지정된 작업을 인스턴스에 추가합니다.`TaskCollection`class. ParentProject.CalculationMode가 None인 경우 사용자는 이 메서드를 사용한 후 Project.Recalculate()를 호출해야 합니다(모든 프로젝트 작업(시작/종료 날짜, 이른/늦은 날짜 설정)을 다시 예약하고 여유 시간, 작업 시간과 같은 종속 필드를 계산합니다. 및 비용 필드, ID 및 개요 수준). ParentProject.CalculationMode가 수동인 경우 메서드는 작업 ID, 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 자동인 경우 메서드는 모든 프로젝트의 작업을 자동으로 다시 예약합니다 (시작/종료) 날짜, 이른/늦은 날짜 설정, 여유 시간 계산, 작업 및 비용 필드, ID 재계산 및 개요 수준). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | 하위 작업 컬렉션에 새 반복 작업을 추가합니다. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | 컬렉션에 지정된 항목이 포함되어 있는지 확인합니다. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | 조상이 이 컬렉션의 상위 작업인 지정된 Id를 가진 작업을 반환합니다. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | 조상이 이 컬렉션의 상위 작업인 지정된 Uid가 있는 작업을 반환합니다. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | 이것은 NotSupportedException 만 throw하는 IList의 Insert 메서드의 스텁 구현입니다. |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | 이것은 NotSupportedException 만 throw하는 ICollection의 Remove 메서드의 스텁 구현입니다. |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | TaskCollection 개체를 다음 목록으로 변환합니다.[`Task`](../task/) 객체. |

### 또한보십시오

* class [Task](../task/)
* 네임스페이스 [Aspose.Tasks](../../aspose.tasks/)
* 집회 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->