---
title: "Kelas ValidationException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ValidationException. Mewakili pengecualian yang dilemparkan ketika kesalahan ditemukan selama validasi entitas"
type: docs
weight: 2790
url: /id/net/aspose.tasks/validationexception/
---
## ValidationException class

Mewakili pengecualian yang dilempar ketika kesalahan ditemukan selama validasi entitas.

```csharp
public class ValidationException : ApplicationException
```

## Contoh

Menampilkan cara menangani &lt;see cref="ValidationException"/&gt; saat bekerja dengan tugas berulang.

```csharp
try
{
    var project = new Project();
    var parameters = new RecurringTaskParameters { TaskName = "t1", Duration = project.GetDuration(1, TimeUnitType.Day), RecurrencePattern = null };
    project.RootTask.Children.Add(parameters);
}
catch (ValidationException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


