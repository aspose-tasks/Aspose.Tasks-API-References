---
title: "Kelas TasksReadingException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TasksReadingException. Mewakili tipe pengecualian pembacaan internal standar"
type: docs
weight: 2540
url: /id/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Mewakili tipe pengecualian pembacaan internal standar.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Mendapatkan informasi pencatatan pengecualian. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Mendapatkan informasi operasi pengecualian. |

## Contoh

Menampilkan cara menangani pengecualian pembacaan/penulisan proyek.

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### Lihat Juga

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


