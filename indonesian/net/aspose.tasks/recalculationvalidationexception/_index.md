---
title: "Class RecalculationValidationException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.RecalculationValidationException. Mewakili pengecualian yang dilempar ketika kesalahan ditemukan dalam proyek setelah perhitungan ulang"
type: docs
weight: 1680
url: /id/net/aspose.tasks/recalculationvalidationexception/
---
## RecalculationValidationException class

Mewakili pengecualian yang dilemparkan ketika kesalahan ditemukan dalam proyek setelah perhitungan ulang.

```csharp
public abstract class RecalculationValidationException : ValidationException
```

## Contoh

Menampilkan pada kondisi apa pengecualian &lt;see cref=\"TaskValidationException\" /&gt; dapat dilempar.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // secara tidak sengaja mengatur tanggal yang salah
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // jalankan perhitungan ulang proyek dengan flag untuk menjalankan validasi
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* class [ValidationException](../validationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


