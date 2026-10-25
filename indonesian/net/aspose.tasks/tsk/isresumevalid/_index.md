---
title: "Tsk.IsResumeValid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas dapat dilanjutkan"
type: docs
weight: 680
url: /id/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Menentukan apakah sebuah tugas dapat dilanjutkan.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsResumeValid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


