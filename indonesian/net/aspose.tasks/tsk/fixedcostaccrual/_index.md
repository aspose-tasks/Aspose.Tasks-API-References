---
title: "Tsk.FixedCostAccrual"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan pilihan bagaimana dan kapan biaya tetap harus dibebankan atau diakumulasi ke biaya sebuah tugas"
type: docs
weight: 440
url: /id/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Menentukan pilihan tentang bagaimana dan kapan biaya tetap harus dibebankan, atau diakumulasi, ke biaya sebuah tugas.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.FixedCostAccrual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


