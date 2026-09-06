---
title: "LoadOptions.Password"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعيّن كلمة مرور الحماية."
type: docs
weight: 50
url: /ar/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

يحصل أو يعيّن كلمة مرور الحماية.

```csharp
public string Password { get; set; }
```

## الأمثلة

يوضح كيفية تحميل المشروع المحمي بكلمة مرور باستخدام &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


