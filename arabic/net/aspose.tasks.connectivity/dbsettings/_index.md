---
title: "فئة DbSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Connectivity.DbSettings. تسمح بتحديد الإعدادات لقراءة من قاعدة بيانات المشروع."
type: docs
weight: 290
url: /ar/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

يسمح بتحديد الإعدادات لقراءة من قاعدة بيانات المشروع.

```csharp
public abstract class DbSettings
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | يحصل أو يعيّن سلسلة الاتصال. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي سيتم استدعاؤه أثناء عمليات تحميل المشروع. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | يحصل أو يعيّن مثيلاً من DbProviderFactory يُستخدم للاتصال بقاعدة البيانات. إذا تم تعيين كل من ProviderFactory و ProviderInvariantName، يكون لـ ProviderFactory أولوية. القيمة الافتراضية هي null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | يحصل أو يعيّن اسم الموفر الثابت الذي يُستخدم للحصول على مثيل من فئة DbProviderFactory. القيمة الافتراضية هي SqlClient. |

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

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


