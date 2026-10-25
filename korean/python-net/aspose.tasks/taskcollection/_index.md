---
title: "TaskCollection"
second_title: "Aspose.Tasks for Python via .NET API 참조"
description: 
type: docs
weight: 1140
url: /ko/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

[Task](/tasks/python-net/aspose.tasks/task/) 객체의 컬렉션을 나타냅니다.

TaskCollection 유형은 다음 멤버를 노출합니다:
## 속성
| 이름 | 설명 |
| :- | :- |
| parent_project | TaskCollection 객체의 상위 프로젝트를 가져옵니다. |
## 메서드
| 이름 | 설명 |
| :- | :- |
| add() | 지정된 작업을 [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) 클래스의 인스턴스에 추가합니다.<br/>            ParentProject.CalculationMode가 None인 경우, 이 메서드 사용 후에 Project.Recalculate()를 호출해야 합니다(모든 프로젝트 작업(시작/완료 날짜)을 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드, ID 및 개요 수준과 같은 종속 필드를 계산합니다).<br/>            ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 ID, 개요 수준 및 개요 번호만 자동으로 계산합니다.<br/>            ParentProject.CalculationMode가 Automatic인 경우, 메서드는 프로젝트의 모든 작업을 자동으로 재조정합니다<br/>            (시작/완료 날짜, 조기/지연 날짜를 설정하고, 여유시간, 작업 및 비용 필드를 계산하며, ID와 개요 수준을 재계산합니다). |
| add(task_name) | 자식 작업 컬렉션에 새 작업을 추가합니다. |
| add(task_name, before_task_id) |  |
| add(parameters) | 지정된 ID를 가진 작업 앞에 새 작업을 삽입하고 동일한 개요 수준에 배치합니다. |
| to_list() | TaskCollection 객체를 [Task](/tasks/python-net/aspose.tasks/task/) 객체 목록으로 변환합니다. |
| get_by_uid(uid) | 이 컬렉션의 상위 작업인 지정된 Uid를 가진 작업을 반환합니다. |
| get_by_id(id) | 이 컬렉션의 상위 작업인 지정된 Id를 가진 작업을 반환합니다. |

### 또 보기

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

