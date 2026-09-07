---
title: "TasksLoggedException.Operation"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TasksLoggedException. Mendapatkan informasi operasi pengecualian"
type: docs
weight: 20
url: /id/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

Mendapatkan informasi operasi pengecualian.

```csharp
public string Operation { get; }
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


