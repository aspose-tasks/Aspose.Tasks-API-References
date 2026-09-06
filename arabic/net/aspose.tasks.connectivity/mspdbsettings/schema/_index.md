---
title: "MspDbSettings.Schema"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MspDbSettings. تحصل أو تعين مخطط خادم MS Project Server. القيمة الافتراضية هي pub"
type: docs
weight: 30
url: /ar/net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

يحصل أو يعيّن مخطط خادم MS Project. القيمة الافتراضية هي "pub".

```csharp
public string Schema { get; set; }
```

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

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


