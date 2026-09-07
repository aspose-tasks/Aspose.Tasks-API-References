---
title: "Kelas TasksLoggedException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TasksLoggedException. Mewakili tipe pengecualian internal standar"
type: docs
weight: 2530
url: /id/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

Mewakili tipe pengecualian internal standar.

```csharp
public class TasksLoggedException : ApplicationException
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


