---
title: "DbSettings.ConnectionString"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "DbSettings प्रॉपर्टी। कनेक्शन स्ट्रिंग प्राप्त करता है या सेट करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

कनेक्शन स्ट्रिंग को प्राप्त करता है या सेट करता है।

```csharp
public string ConnectionString { get; set; }
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


