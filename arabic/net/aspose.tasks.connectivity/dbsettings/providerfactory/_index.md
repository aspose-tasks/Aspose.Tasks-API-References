---
title: "DbSettings.ProviderFactory"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية DbSettings. تحصل أو تعين مثيلًا من DbProviderFactory يُستخدم للاتصال بقاعدة البيانات. إذا تم تعيين كل من ProviderFactory و ProviderInvariantName فإن ProviderFactory له أولوية. القيمة الافتراضية هي null"
type: docs
weight: 30
url: /ar/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

يحصل أو يعيّن مثيلاً من DbProviderFactory يُستخدم للاتصال بقاعدة البيانات. إذا تم تعيين كل من ProviderFactory و ProviderInvariantName، يكون لـ ProviderFactory أولوية. القيمة الافتراضية هي null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


