---
title: "TasksLoggedException.LogText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TasksLoggedException. Mendapatkan informasi pencatatan pengecualian"
type: docs
weight: 10
url: /id/net/aspose.tasks/tasksloggedexception/logtext/
---
## TasksLoggedException.LogText property

Mendapatkan informasi pencatatan pengecualian.

```csharp
public string LogText { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


