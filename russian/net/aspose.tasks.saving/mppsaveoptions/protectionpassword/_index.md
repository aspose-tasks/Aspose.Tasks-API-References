---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MPPSaveOptions. Возвращает или задает пароль, используемый для защиты получаемого файла MPP. В настоящее время поддерживается для форматов MS Project 2010 и новее. Значение null указывает, что файл проекта не защищён."
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

Получает или задает пароль, используемый для защиты получаемого файла MPP. В настоящее время поддерживается для форматов MS Project 2010 и новее. Значение null указывает, что файл проекта не защищён.

```csharp
public string ProtectionPassword { get; set; }
```

## Примеры

Показывает, как сохранить проект в защищённый паролем файл MPP.

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

### См. также

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


