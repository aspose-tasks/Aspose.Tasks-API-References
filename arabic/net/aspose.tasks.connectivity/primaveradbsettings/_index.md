---
title: "فئة PrimaveraDbSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Connectivity.PrimaveraDbSettings. تسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من قاعدة بيانات Primavera."
type: docs
weight: 320
url: /ar/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

يسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من قاعدة بيانات Primavera.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | ينشئ مثيلاً جديداً من الفئة `PrimaveraDbSettings`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | يحصل أو يعيّن سلسلة الاتصال. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | يحصل على معرف المشروع المراد قراءته. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي سيتم استدعاؤه أثناء عمليات تحميل المشروع. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | يحصل أو يعيّن مثيلاً من DbProviderFactory يُستخدم للاتصال بقاعدة البيانات. إذا تم تعيين كل من ProviderFactory و ProviderInvariantName، يكون لـ ProviderFactory أولوية. القيمة الافتراضية هي null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | يحصل أو يعيّن اسم الموفر الثابت الذي يُستخدم للحصول على مثيل من فئة DbProviderFactory. القيمة الافتراضية هي SqlClient. |

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

يظهر كيفية الحصول على معلومات مختصرة للمشاريع من قاعدة بيانات Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### انظر أيضًا

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


