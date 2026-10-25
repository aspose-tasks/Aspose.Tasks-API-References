---
title: "Tsk.IsRecurring"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas merupakan bagian dari rangkaian tugas berulang"
type: docs
weight: 670
url: /id/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Menentukan apakah sebuah tugas merupakan bagian dari serangkaian tugas berulang.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsRecurring.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


