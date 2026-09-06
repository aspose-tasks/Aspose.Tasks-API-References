---
title: "MPPSaveOptions.ProtectionPassword"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MPPSaveOptions. تحصل أو تعين كلمة مرور تُستخدم لحماية ملف MPP الناتج. مدعوم حاليًا لتنسيقات MS Project 2010 والأحدث. القيمة Null تشير إلى أن ملف المشروع غير محمي."
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/mppsaveoptions/protectionpassword/
---
## MPPSaveOptions.ProtectionPassword property

يحصل أو يعيّن كلمة مرور تُستخدم لحماية ملف MPP الناتج. حاليًا يتم دعم ذلك لتنسيقات MS Project 2010 وما بعدها. القيمة Null تشير إلى أن ملف المشروع غير محمي.

```csharp
public string ProtectionPassword { get; set; }
```

## الأمثلة

يوضح كيفية حفظ مشروع إلى ملف MPP محمي بكلمة مرور.

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

### انظر أيضًا

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


