---
title: "क्लास MpdSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Connectivity.MpdSettings क्लास। MPD फ़ॉर्मेट MS Access डेटाबेस फ़ाइल फ़ॉर्मेट से प्रोजेक्ट डेटा पढ़ने के लिए आवश्यक विकल्प सेट करने की अनुमति देता है।"
type: docs
weight: 300
url: /hi/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

MPD फ़ॉर्मेट (MS Access डेटाबेस फ़ाइल फ़ॉर्मेट) से प्रोजेक्ट डेटा पढ़ने के लिए आवश्यक विकल्प सेट करने की अनुमति देता है।

```csharp
public class MpdSettings : DbSettings
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | `MpdSettings` क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | कनेक्शन स्ट्रिंग को प्राप्त करता है या सेट करता है। |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | पढ़ने के लिए प्रोजेक्ट का आईडी प्राप्त करता है। |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | प्रोजेक्ट लोडिंग ऑपरेशन्स के दौरान कॉल किया जाने वाला कॉलबैक प्राप्त करता है या सेट करता है। |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | DB से कनेक्ट करने के लिए उपयोग की जाने वाली DbProviderFactory का एक इंस्टेंस प्राप्त करता है या सेट करता है। यदि दोनों ProviderFactory और ProviderInvariantName सेट हैं, तो ProviderFactory को प्राथमिकता मिलती है। डिफ़ॉल्ट मान null है। |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | DbProviderFactory क्लास का इंस्टेंस प्राप्त करने के लिए उपयोग किए जाने वाले प्रोवाइडर इनवेरिएंट नाम को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान SqlClient है। |

## उदाहरण

डेटाबेस से प्रोजेक्ट इम्पोर्ट को नियंत्रित करने के लिए MPD सेटिंग्स का उपयोग कैसे करें, यह दिखाता है।

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


