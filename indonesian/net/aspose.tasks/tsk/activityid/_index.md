---
title: "Tsk.ActivityId"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Mewakili bidang ID aktivitas, pengidentifikasi unik tugas yang digunakan oleh Primavera. hanya berlaku untuk proyek Primavera"
type: docs
weight: 10
url: /id/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Mewakili bidang id aktivitas - pengidentifikasi unik sebuah tugas yang digunakan oleh Primavera. (hanya berlaku untuk proyek Primavera).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Contoh

Menampilkan cara bekerja dengan bidang ActivityId khusus untuk proyek Primavera

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// buat opsi penyimpanan Primavera dan tentukan bahwa ActivityIds tidak boleh ditimpa selama penyimpanan.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


