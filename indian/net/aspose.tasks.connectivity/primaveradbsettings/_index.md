---
title: "क्लास PrimaveraDbSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Connectivity.PrimaveraDbSettings क्लास। Primavera डेटाबेस से प्रोजेक्ट डेटा पढ़ने के लिए आवश्यक विकल्प सेट करने की अनुमति देता है।"
type: docs
weight: 320
url: /hi/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Primavera डेटाबेस से प्रोजेक्ट डेटा पढ़ने के लिए आवश्यक विकल्प सेट करने की अनुमति देता है।

```csharp
public class PrimaveraDbSettings : DbSettings
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | `PrimaveraDbSettings` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | कनेक्शन स्ट्रिंग को प्राप्त करता है या सेट करता है। |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | पढ़ने के लिए प्रोजेक्ट का आईडी प्राप्त करता है। |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | प्रोजेक्ट लोडिंग ऑपरेशन्स के दौरान कॉल किया जाने वाला कॉलबैक प्राप्त करता है या सेट करता है। |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | DB से कनेक्ट करने के लिए उपयोग की जाने वाली DbProviderFactory का एक इंस्टेंस प्राप्त करता है या सेट करता है। यदि दोनों ProviderFactory और ProviderInvariantName सेट हैं, तो ProviderFactory को प्राथमिकता मिलती है। डिफ़ॉल्ट मान null है। |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory क्लास का इंस्टेंस प्राप्त करने के लिए उपयोग किए जाने वाले प्रोवाइडर इनवेरिएंट नाम को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान SqlClient है। |

## उदाहरण

Primavera डेटाबेस से प्रोजेक्ट इम्पोर्ट करने का तरीका दिखाता है।

```csharp
// कनेक्शन स्ट्रिंग और प्रोजेक्ट आईडी के साथ PrimaveraDbSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करें
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// UID = 4502 के साथ प्रोजेक्ट पढ़ें
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

Primavera डेटाबेस से परियोजनाओं की संक्षिप्त जानकारी कैसे प्राप्त करें, यह दर्शाता है।

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

### संबंधित देखें

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


