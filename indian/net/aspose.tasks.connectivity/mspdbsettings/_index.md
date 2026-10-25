---
title: "क्लास MspDbSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Connectivity.MspDbSettings क्लास। प्रोजेक्ट डेटा को MS Project Server डेटाबेस से पढ़ने के लिए आवश्यक विकल्प सेट करने की अनुमति देता है"
type: docs
weight: 310
url: /hi/net/aspose.tasks.connectivity/mspdbsettings/
---
## MspDbSettings class

MS Project Server डेटाबेस से प्रोजेक्ट डेटा पढ़ने के लिए आवश्यक विकल्प सेट करने की अनुमति देता है।

```csharp
public class MspDbSettings : DbSettings
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [MspDbSettings](mspdbsettings/)(string, Guid) | `MspDbSettings` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | कनेक्शन स्ट्रिंग को प्राप्त करता है या सेट करता है। |
| [ProjectGuid](../../aspose.tasks.connectivity/mspdbsettings/projectguid/) { get; } | पढ़ने के लिए प्रोजेक्ट का GUID प्राप्त करता है। |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | प्रोजेक्ट लोडिंग ऑपरेशन्स के दौरान कॉल किया जाने वाला कॉलबैक प्राप्त करता है या सेट करता है। |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | DB से कनेक्ट करने के लिए उपयोग की जाने वाली DbProviderFactory का एक इंस्टेंस प्राप्त करता है या सेट करता है। यदि दोनों ProviderFactory और ProviderInvariantName सेट हैं, तो ProviderFactory को प्राथमिकता मिलती है। डिफ़ॉल्ट मान null है। |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory क्लास का इंस्टेंस प्राप्त करने के लिए उपयोग किए जाने वाले प्रोवाइडर इनवेरिएंट नाम को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान SqlClient है। |
| [Schema](../../aspose.tasks.connectivity/mspdbsettings/schema/) { get; set; } | MS Project Server का स्कीमा प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान "pub" है। |

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

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


