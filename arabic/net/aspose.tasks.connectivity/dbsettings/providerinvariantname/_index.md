---
title: "DbSettings.ProviderInvariantName"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية DbSettings. تحصل أو تعين اسم الموفر الثابت الذي يُستخدم للحصول على مثيل من فئة DbProviderFactory. القيمة الافتراضية هي SqlClient"
type: docs
weight: 40
url: /ar/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

يحصل أو يعيّن اسم الموفر الثابت الذي يُستخدم للحصول على مثيل من فئة DbProviderFactory. القيمة الافتراضية هي SqlClient.

```csharp
public string ProviderInvariantName { get; set; }
```

## الأمثلة

يوضح كيفية قراءة مشروع من ملف Primavera XML يحتوي على مشاريع متعددة باستخدام اسم موفر.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// إنشاء إعدادات قاعدة بيانات Primavera باستخدام سلسلة الاتصال ومعرف المشروع
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


