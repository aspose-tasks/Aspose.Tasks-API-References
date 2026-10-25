---
title: "الفئة MspDbSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Connectivity.MspDbSettings. تسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من قاعدة بيانات خادم MS Project"
type: docs
weight: 310
url: /ar/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

يسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من قاعدة بيانات خادم MS Project.

```csharp
public class MspDbSettings : DbSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | ينشئ مثيلاً جديداً من الفئة `MspDbSettings`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | يحصل أو يعيّن سلسلة الاتصال. |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | يحصل على الـ guid للمشروع المراد قراءته. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي سيتم استدعاؤه أثناء عمليات تحميل المشروع. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | يحصل أو يعيّن مثيلاً من DbProviderFactory يُستخدم للاتصال بقاعدة البيانات. إذا تم تعيين كل من ProviderFactory و ProviderInvariantName، يكون لـ ProviderFactory أولوية. القيمة الافتراضية هي null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | يحصل أو يعيّن اسم الموفر الثابت الذي يُستخدم للحصول على مثيل من فئة DbProviderFactory. القيمة الافتراضية هي SqlClient. |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | يحصل أو يعيّن مخطط خادم MS Project. القيمة الافتراضية هي "pub". |

## الأمثلة

يوضح كيفية استيراد مشروع من قاعدة بيانات.

```csharp
try
{
    // إنشاء سلسلة الاتصال
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // إنشاء إعدادات للتحميل من قاعدة بيانات MS
    var settings = new MspDbSettings(connectionString.ConnectionString, new Guid("E6426C44-D6CB-4B9C-AF16-48910ACE0F54"));
    settings.Schema = "dbo";

    Console.WriteLine("Project GUID to load: " + settings.ProjectGuid);

    var project = new Project(settings);

    project.Save(OutDir + "ImportProjectDataFromDatabase_out.mpp", SaveFileFormat.Mpp);
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message + " Please setup proper data source (DataSource, InitialCatalog etc)");
}
```

### انظر أيضًا

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


