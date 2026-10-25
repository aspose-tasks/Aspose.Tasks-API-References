---
title: "Kelas TasksWritingException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TasksWritingException. Mewakili tipe pengecualian penulisan internal standar."
type: docs
weight: 2560
url: /id/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

Mewakili tipe pengecualian penulisan internal standar.

```csharp
public class TasksWritingException : TasksLoggedException
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Mendapatkan informasi pencatatan pengecualian. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Mendapatkan informasi operasi pengecualian. |

## Contoh

Menampilkan cara membaca teks log dan jenis pengecualian untuk memeriksa masalah dengan ekspor MPP.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // ekspor proyek sebagai file MPP
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### Lihat Juga

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


