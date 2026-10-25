---
title: "Kelas TasksException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TasksException. Mewakili tipe pengecualian internal standar."
type: docs
weight: 2520
url: /id/net/aspose.tasks/tasksexception/
---
## TasksException class

Mewakili tipe pengecualian internal standar.

```csharp
public class TasksException : ApplicationException
```

## Contoh

Menampilkan cara mendeteksi struktur proyek yang rusak.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// periksa struktur proyek.
// Jika struktur proyek tidak benar, <see cref="TasksException"> akan dilemparkan.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


