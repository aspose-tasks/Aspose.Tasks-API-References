---
title: "क्लास DbSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Connectivity.DbSettings क्लास। प्रोजेक्ट डेटाबेस से पढ़ने के लिए सेटिंग्स निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 290
url: /hi/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

प्रोजेक्ट डेटाबेस से पढ़ने के लिए सेटिंग्स निर्दिष्ट करने की अनुमति देता है।

```csharp
public abstract class DbSettings
```

## गुण

| नाम | विवरण |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | कनेक्शन स्ट्रिंग को प्राप्त करता है या सेट करता है। |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | प्रोजेक्ट लोडिंग ऑपरेशन्स के दौरान कॉल किया जाने वाला कॉलबैक प्राप्त करता है या सेट करता है। |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | DB से कनेक्ट करने के लिए उपयोग की जाने वाली DbProviderFactory का एक इंस्टेंस प्राप्त करता है या सेट करता है। यदि दोनों ProviderFactory और ProviderInvariantName सेट हैं, तो ProviderFactory को प्राथमिकता मिलती है। डिफ़ॉल्ट मान null है। |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory क्लास का इंस्टेंस प्राप्त करने के लिए उपयोग किए जाने वाले प्रोवाइडर इनवेरिएंट नाम को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान SqlClient है। |

## उदाहरण

प्रोवाइडर नाम का उपयोग करके कई प्रोजेक्ट्स वाले Primavera XML फ़ाइल से प्रोजेक्ट पढ़ने का तरीका दिखाता है।

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// कनेक्शन स्ट्रिंग और प्रोजेक्ट आईडी का उपयोग करके Primavera DB सेटिंग्स बनाएं
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


