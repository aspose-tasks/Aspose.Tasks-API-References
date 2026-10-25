---
title: "Kelas InvalidPasswordException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.InvalidPasswordException. Mewakili tipe pengecualian yang dilempar ketika membuka file yang dilindungi kata sandi dengan kata sandi yang salah."
type: docs
weight: 910
url: /id/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Mewakili tipe pengecualian yang dilemparkan ketika membuka file yang dilindungi kata sandi dengan kata sandi yang salah.

```csharp
public class InvalidPasswordException : TasksException
```

## Contoh

Menampilkan cara menangani &lt;see cref="InvalidPasswordException"/&gt; saat membaca file proyek yang dilindungi kata sandi.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // bekerja dengan proyek ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // pesannya adalah "Proyek dilindungi kata sandi. Kata sandi tidak diberikan atau salah."
    Console.WriteLine(e.Message);
}
```

### Lihat Juga

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


