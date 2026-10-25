---
title: "Tsk.IsNull"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Menentukan apakah sebuah tugas adalah tugas null"
type: docs
weight: 640
url: /id/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Menentukan apakah sebuah tugas adalah tugas null.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IsNull.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


