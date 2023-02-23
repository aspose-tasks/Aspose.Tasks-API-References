---
title: Project.Recalculate
second_title: Aspose.Tasks for .NET API 参考
description: Project 方法. 重新安排所有项目任务 ID大纲级别开始/结束日期设置早/晚日期计算松弛时间工时和成本字段
type: docs
weight: 1120
url: /zh/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

重新安排所有项目任务 ID、大纲级别、开始/结束日期、设置早/晚日期、计算松弛时间、工时和成本字段。

```csharp
public void Recalculate()
```

### 也可以看看

* class [Project](../)
* 命名空间 [Aspose.Tasks](../../project/)
* 部件 [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

重新安排所有项目任务 ID、大纲级别、开始/结束日期、设置早/晚日期、计算松弛时间、工作和成本字段以及可选验证。

```csharp
public void Recalculate(bool validate)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| validate | Boolean | 如果为真，将执行重新计算的验证。 验证哪些数据： 目前仅实现任务和任务链接日期范围的基本验证。 任务的日期范围（例如 ActualStart - ActualFinish、EarlyStart - EarlyFinish 等。 ) 以及任务链接日期将根据开始日期小于或等于完成日期的日期标准进行检查。 如果上述任何条件失败，则[`RecalculationValidationException`](../../recalculationvalidationexception/)将被抛出. |

### 也可以看看

* class [Project](../)
* 命名空间 [Aspose.Tasks](../../project/)
* 部件 [Aspose.Tasks](../../../)


