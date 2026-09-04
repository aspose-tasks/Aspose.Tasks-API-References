---
title: "TaskStatus"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定任务的状态。"
type: docs
weight: 301
url: /zh/java/com.aspose.tasks/taskstatus/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TaskStatus extends System.Enum
```

指定任务的状态。
## 字段

| 字段 | 描述 |
| --- | --- |
| [Complete](#Complete) | 任务已完成 100%。 |
| [Future](#Future) | 'Future' 任务状态在任务开始日期大于状态日期时设置。 |
| [Late](#Late) | 如果 timephased 累计完成百分比在状态日期前一天未达到午夜，任务将迟延。 |
| [OnSchedule](#OnSchedule) | 如果 timephased 累计完成百分比至少覆盖到状态日期前一天，任务按计划进行。 |
| [Undefined](#Undefined) | 未定义的任务状态。 |
### Complete {#Complete}
```
public static final int Complete
```


任务已完成 100%。

### Future {#Future}
```
public static final int Future
```


'Future' 任务状态在任务开始日期大于状态日期时设置。

### Late {#Late}
```
public static final int Late
```


如果 timephased 累计完成百分比在状态日期前一天未达到午夜，任务将迟延。

### OnSchedule {#OnSchedule}
```
public static final int OnSchedule
```


如果 timephased 累计完成百分比至少覆盖到状态日期前一天，任务按计划进行。

### Undefined {#Undefined}
```
public static final int Undefined
```


未定义的任务状态。

