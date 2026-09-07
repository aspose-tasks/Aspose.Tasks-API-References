---
title: "MspDbSettings.MspDbSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MspDbSettings कंस्ट्रक्टर। MspDbSettings क्लास का एक नया उदाहरण इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.connectivity/mspdbsettings/mspdbsettings/
---
## MspDbSettings constructor

[`MspDbSettings`](../) क्लास का एक नया उदाहरण इनिशियलाइज़ करता है।

```csharp
public MspDbSettings(string connectionString, Guid projectGuid)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| connectionString | स्ट्रिंग | निर्दिष्ट कनेक्शन स्ट्रिंग। |
| projectGuid | Guid | पढ़ने के लिए प्रोजेक्ट का निर्दिष्ट GUID। |

## उदाहरण

डेटाबेस से प्रोजेक्ट इम्पोर्ट करने का तरीका दिखाता है।

```csharp
try
{
    // कनेक्शन स्ट्रिंग बनाएं
    var connectionString = new SqlConnectionStringBuilder();
    connectionString.DataSource = "192.168.56.2,1433";
    connectionString.Encrypt = true;
    connectionString.TrustServerCertificate = true;
    connectionString.InitialCatalog = "ProjectServer_Published";
    connectionString.NetworkLibrary = "DBMSSOCN";
    connectionString.UserID = "sa";
    connectionString.Password = "*****";

    // MS डेटाबेस से लोड करने के लिए सेटिंग्स बनाएं
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

### संबंधित देखें

* class [MspDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mspdbsettings/)
* assembly [Aspose.Tasks](../../../)


