---
title: "PrimaveraDbSettings.ProjectId"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraDbSettings. تحصل على معرف المشروع للقراءة"
type: docs
weight: 20
url: /ar/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

يحصل على معرف المشروع المراد قراءته.

```csharp
public int ProjectId { get; }
```

## الأمثلة

يوضح كيفية استيراد مشروع من قاعدة بيانات Primavera.

```csharp
// إنشاء مثيل جديد من فئة PrimaveraDbSettings باستخدام سلسلة الاتصال ومعرف المشروع
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// قراءة المشروع بمعرف UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### انظر أيضًا

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


