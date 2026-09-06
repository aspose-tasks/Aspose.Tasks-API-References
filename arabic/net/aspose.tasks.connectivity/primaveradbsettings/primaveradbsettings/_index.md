---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PrimaveraDbSettings. يهيئ مثيلًا جديدًا من الفئة PrimaveraDbSettings"
type: docs
weight: 10
url: /ar/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

يهيئ مثيلًا جديدًا من الفئة [`PrimaveraDbSettings`](../).

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| connectionString | سلسلة | سلسلة الاتصال المحددة. |
| projectId | Int32 | المعرف المحدد لمشروع للقراءة. |

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


