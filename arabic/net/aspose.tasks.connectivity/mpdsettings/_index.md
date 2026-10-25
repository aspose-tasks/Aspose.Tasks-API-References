---
title: "فئة MpdSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Connectivity.MpdSettings. تسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من تنسيق MPD لملف قاعدة بيانات MS Access."
type: docs
weight: 300
url: /ar/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

يسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من تنسيق MPD (تنسيق ملف قاعدة بيانات MS Access).

```csharp
public class MpdSettings : DbSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | ينشئ مثيلاً جديداً من الفئة `MpdSettings`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | يحصل أو يعيّن سلسلة الاتصال. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | يحصل على معرف المشروع المراد قراءته. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي سيتم استدعاؤه أثناء عمليات تحميل المشروع. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | يحصل أو يعيّن مثيلاً من DbProviderFactory يُستخدم للاتصال بقاعدة البيانات. إذا تم تعيين كل من ProviderFactory و ProviderInvariantName، يكون لـ ProviderFactory أولوية. القيمة الافتراضية هي null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | يحصل أو يعيّن اسم الموفر الثابت الذي يُستخدم للحصول على مثيل من فئة DbProviderFactory. القيمة الافتراضية هي SqlClient. |

## الأمثلة

يوضح كيفية استخدام إعدادات MPD للتحكم في استيراد المشروع من قاعدة البيانات.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


