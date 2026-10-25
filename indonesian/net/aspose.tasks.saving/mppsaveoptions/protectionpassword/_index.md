---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti MPPSaveOptions. Mendapatkan atau mengatur kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan. Saat ini didukung untuk format MS Project 2010 dan yang lebih baru. Nilai null menunjukkan bahwa file proyek tidak dilindungi."
type: docs
weight: 30
url: /id/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Mendapatkan atau mengatur kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan. Saat ini didukung untuk format MS Project 2010 dan yang lebih baru. Nilai null menunjukkan bahwa file proyek tidak dilindungi.

```csharp
public string ProtectionPassword { get; set; }
```

## Contoh

Menampilkan cara menyimpan proyek ke file MPP yang dilindungi kata sandi.

```csharp
try
{

    var project = new Project(DataDir + "Project1.mpp");

    SimpleSaveOptions options = new MPPSaveOptions
    {
        ProtectionPassword = "password!234"
    };

    project.Save(OutDir + "PasswordProtected.mpp", options);
}
catch (NotSupportedException ex)
{
    Console.WriteLine(ex.Message + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
}
```

### Lihat Juga

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


