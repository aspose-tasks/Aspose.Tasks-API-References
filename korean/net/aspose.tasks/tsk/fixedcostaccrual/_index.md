---
title: "Tsk.FixedCostAccrual"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 고정 비용을 언제, 어떻게 작업 비용에 청구하거나 발생시킬지를 선택합니다."
type: docs
weight: 440
url: /ko/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

고정 비용을 작업 비용에 청구하거나 발생시킬 시기와 방법에 대한 선택을 결정합니다.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## 예제

Tsk.FixedCostAccrual 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


