---
title: "DbSettings.ProviderInvariantName"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "DbSettings प्रॉपर्टी। प्रोवाइडर इनवेरिएंट नाम प्राप्त करता है या सेट करता है, जिसका उपयोग DbProviderFactory क्लास का एक इंस्टेंस प्राप्त करने के लिए किया जाता है। डिफ़ॉल्ट मान है SqlClient"
type: docs
weight: 40
url: /hi/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

DbProviderFactory क्लास का इंस्टेंस प्राप्त करने के लिए उपयोग किए जाने वाले प्रोवाइडर इनवेरिएंट नाम को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान SqlClient है।

```csharp
public string ProviderInvariantName { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


