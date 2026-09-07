---
title: "MspDbSettings.Schema"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MspDbSettings प्रॉपर्टी। MS Project Server का स्कीमा प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान है pub"
type: docs
weight: 30
url: /hi/net/aspose.tasks.connectivity/mspdbsettings/schema/
---
## MspDbSettings.Schema property

MS Project Server का स्कीमा प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान "pub" है।

```csharp
public string Schema { get; set; }
```

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


