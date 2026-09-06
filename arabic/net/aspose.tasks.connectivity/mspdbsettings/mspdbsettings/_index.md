---
title: "MspDbSettings.MspDbSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ MspDbSettings. يهيئ مثيلاً جديداً من فئة MspDbSettings"
type: docs
weight: 10
url: /ar/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

يهيئ مثيلاً جديداً من فئة [`MspDbSettings`](../).

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| connectionString | سلسلة | سلسلة الاتصال المحددة. |
| projectGuid | Guid | معرف GUID المحدد لمشروع للقراءة. |

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


