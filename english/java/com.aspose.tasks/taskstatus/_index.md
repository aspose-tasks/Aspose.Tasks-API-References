---
title: TaskStatus
second_title: Aspose.Tasks for Java API Reference
description: Specifies the status of a task.
type: docs
weight: 300
url: /java/com.aspose.tasks/taskstatus/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TaskStatus extends System.Enum
```

Specifies the status of a task.
## Fields

| Field | Description |
| --- | --- |
| [Complete](#Complete) | The task is 100 percent complete. |
| [Future](#Future) | 'Future' task status is set when the task start date is greater than the status date. |
| [Late](#Late) | The task is late if the timephased cumulative percent complete does not reach midnight on the day before the status date. |
| [OnSchedule](#OnSchedule) | The task is on schedule if timephased cumulative percent complete is spread to at least the day before the status date. |
| [Undefined](#Undefined) | Undefined task status. |
### Complete {#Complete}
```
public static final int Complete
```


The task is 100 percent complete.

### Future {#Future}
```
public static final int Future
```


'Future' task status is set when the task start date is greater than the status date.

### Late {#Late}
```
public static final int Late
```


The task is late if the timephased cumulative percent complete does not reach midnight on the day before the status date.

### OnSchedule {#OnSchedule}
```
public static final int OnSchedule
```


The task is on schedule if timephased cumulative percent complete is spread to at least the day before the status date.

### Undefined {#Undefined}
```
public static final int Undefined
```


Undefined task status.

