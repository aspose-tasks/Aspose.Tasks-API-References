---
title: Add
second_title: .NET API 참조용 Aspose.Tasks
description: 지정된 작업을 인스턴스에 추가합니다.TaskCollectionaspose.tasks/taskcollection/class. ParentProject.CalculationMode가 None인 경우 사용자는 이 메서드를 사용한 후 Project.Recalculate를 호출해야 합니다모든 프로젝트 작업시작/종료 날짜 이른/늦은 날짜 설정을 다시 예약하고 여유 시간 작업 시간과 같은 종속 필드를 계산합니다. 및 비용 필드 ID 및 개요 수준. ParentProject.CalculationMode가 수동인 경우 메서드는 작업 ID 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 자동인 경우 메서드는 모든 프로젝트의 작업을 자동으로 다시 예약합니다 시작/종료 날짜 이른/늦은 날짜 설정 여유 시간 계산 작업 및 비용 필드 ID 재계산 및 개요 수준.
type: docs
weight: 50
url: /ko/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

지정된 작업을 인스턴스에 추가합니다.[`TaskCollection`](../)class. ParentProject.CalculationMode가 None인 경우 사용자는 이 메서드를 사용한 후 Project.Recalculate()를 호출해야 합니다(모든 프로젝트 작업(시작/종료 날짜, 이른/늦은 날짜 설정)을 다시 예약하고 여유 시간, 작업 시간과 같은 종속 필드를 계산합니다. 및 비용 필드, ID 및 개요 수준). ParentProject.CalculationMode가 수동인 경우 메서드는 작업 ID, 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 자동인 경우 메서드는 모든 프로젝트의 작업을 자동으로 다시 예약합니다 (시작/종료) 날짜, 이른/늦은 날짜 설정, 여유 시간 계산, 작업 및 비용 필드, ID 재계산 및 개요 수준).

```csharp
public void Add(Task item)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| item | Task | 이 작업 모음에 추가해야 하는 지정된 작업입니다. |

### 또한보십시오

* class [Task](../../task/)
* class [TaskCollection](../)
* 네임스페이스 [Aspose.Tasks](../../taskcollection/)
* 집회 [Aspose.Tasks](../../../)

---

## Add() {#add}

마지막 작업과 동일한 개요 수준에서 프로젝트 작업 컬렉션에 새 작업을 추가합니다.

```csharp
public Task Add()
```

### 반환 값

의 새로 추가된 인스턴스를 반환합니다.[`Task`](../../task/) 수업.

### 또한보십시오

* class [Task](../../task/)
* class [TaskCollection](../)
* 네임스페이스 [Aspose.Tasks](../../taskcollection/)
* 집회 [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

자식 작업 컬렉션에 새 작업을 추가합니다.

```csharp
public Task Add(string taskName)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| taskName | String | 지정된 작업 이름. |

### 반환 값

의 새로 추가된 인스턴스를 반환합니다.[`Task`](../../task/) 수업.

### 또한보십시오

* class [Task](../../task/)
* class [TaskCollection](../)
* 네임스페이스 [Aspose.Tasks](../../taskcollection/)
* 집회 [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

하위 작업 컬렉션에 새 반복 작업을 추가합니다.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| taskName | String | 지정된 작업 이름. |
| beforeTaskId | Int32 | 새 작업이 삽입되기 전에 작업의 지정된 ID입니다. |

### 반환 값

지정된 ID를 가진 작업 앞에 삽입된 작업을 반환합니다.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | 지정된 ID가 유효한 작업 ID가 아닌 경우 ArgumentOutOfRangeException이 발생합니다. |

### 또한보십시오

* class [Task](../../task/)
* class [TaskCollection](../)
* 네임스페이스 [Aspose.Tasks](../../taskcollection/)
* 집회 [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

동일한 개요 수준에서 지정된 ID를 가진 작업 앞에 새 작업을 삽입합니다.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| parameters | RecurringTaskParameters | 매개변수는 반복 작업 생성을 위해 지정된 매개변수입니다. |

### 반환 값

의 새로 추가된 인스턴스를 반환합니다.[`Task`](../../task/) 수업.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | 지정된 매개변수가 null인 경우 발생합니다. |
| ArgumentException | 지정된 매개변수가 유효하지 않은 경우 발생합니다. |

### 또한보십시오

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* 네임스페이스 [Aspose.Tasks](../../taskcollection/)
* 집회 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
