---
title: Project.RescheduleUncompletedWorkToStartAfter
second_title: Справочник по Aspose.Tasks для .NET API
description: Project метод. Перепланирует незавершенную проектную работу так чтобы она началась после указанной даты.
type: docs
weight: 1170
url: /ru/net/aspose.tasks/project/rescheduleuncompletedworktostartafter/
---
## RescheduleUncompletedWorkToStartAfter(DateTime) {#rescheduleuncompletedworktostartafter}

Перепланирует незавершенную проектную работу так, чтобы она началась после указанной даты.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| after | DateTime | Дата переноса незавершенной работы после. |

### Примечания

Перед использованием этого метода убедитесь, что для флага Project.CanSplitsInProgressTasks установлено значение true.

### Смотрите также

* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)

---

## RescheduleUncompletedWorkToStartAfter(DateTime, List&lt;Task&gt;) {#rescheduleuncompletedworktostartafter_1}

Перепланирует незавершенную работу для указанного списка задач, чтобы начать ее после указанной даты.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after, List<Task> taskCollection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| after | DateTime | Дата переноса незавершенной работы после. |
| taskCollection | List`1 | Список&lt;Task&gt; задач, для которых необходимо перепланировать незавершенную работу. |

### Примечания

Перед использованием этого метода убедитесь, что для флага Project.CanSplitsInProgressTasks установлено значение true.

### Смотрите также

* class [Task](../../task/)
* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)


