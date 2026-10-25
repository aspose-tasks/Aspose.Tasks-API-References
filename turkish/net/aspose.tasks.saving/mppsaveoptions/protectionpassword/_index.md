---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MPPSaveOptions özelliği. Oluşan MPP dosyasını korumak için kullanılan bir şifreyi alır veya ayarlar. Şu anda MS Project 2010 ve daha yeni formatlar için desteklenmektedir. Null değeri, proje dosyasının korunmadığını gösterir."
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Oluşturulan MPP dosyasını korumak için kullanılan bir parolayı alır veya ayarlar. Şu anda MS Project 2010 ve daha yeni formatlar için desteklenmektedir. Null değeri, proje dosyasının korunmadığını gösterir.

```csharp
public string ProtectionPassword { get; set; }
```

## Örnekler

Bir projeyi şifre korumalı MPP dosyasına nasıl kaydedeceğinizi gösterir.

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

### Ayrıca Bakınız

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


