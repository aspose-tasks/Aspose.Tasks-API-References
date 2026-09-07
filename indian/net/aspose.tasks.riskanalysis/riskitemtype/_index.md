---
title: "एन्यूम RiskItemType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RiskAnalysis.RiskItemType एन्यूम। उन टास्क फ़ील्ड्स को निर्दिष्ट करता है जिनके लिए जोखिम विश्लेषण के दौरान सांख्यिकीय जानकारी एकत्र की जाती है।"
type: docs
weight: 1920
url: /hi/net/aspose.tasks.riskanalysis/riskitemtype/
---
## RiskItemType enumeration

जो कार्य फ़ील्ड हैं, जिनके लिए जोखिम विश्लेषण के दौरान सांख्यिकीय जानकारी एकत्र की जाती है, उन्हें निर्दिष्ट करता है।

```csharp
public enum RiskItemType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Start | `0` | कार्य प्रारम्भ। |
| Finish | `1` | कार्य समाप्ति। |
| EarlyStart | `2` | कार्य शीघ्र प्रारम्भ। |
| EarlyFinish | `3` | कार्य शीघ्र समाप्ति। |
| LateStart | `4` | कार्य देर से प्रारम्भ। |
| LateFinish | `5` | कार्य देर से समाप्ति। |

## उदाहरण

दिखाता है कि जोखिमों के आँकड़े कैसे गणना करें और उन्हें PDF रिपोर्ट के रूप में कैसे सेव करें।

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// एक जोखिम पैटर्न प्रारंभ करें
var pattern = new RiskPattern(task)
{
    // रैंडम नंबर जेनरेटर के लिए एक वितरण प्रकार चुनें जिससे संभावित मान उत्पन्न हों (वर्तमान में केवल दो प्रकार समर्थित हैं, अर्थात सामान्य और समान)।
    // अधिक विवरण के लिए यहाँ देखें: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // सबसे संभावित कार्य अवधि का प्रतिशत सेट करें जो सर्वोत्तम प्रोजेक्ट परिदृश्य में हो सकता है
    // डिफ़ॉल्ट मान 75 है, जिसका अर्थ है कि यदि अनुमानित कार्य अवधि 4 दिन है तो आशावादी अवधि 3 दिन होगी
    Optimistic = 70,

    // सबसे संभावित कार्य अवधि का प्रतिशत सेट करें जो सबसे खराब प्रोजेक्ट परिदृश्य में हो सकता है
    // डिफ़ॉल्ट मान 125 है, जिसका अर्थ है कि यदि अनुमानित कार्य अवधि 4 दिन है तो निराशावादी अवधि 5 दिन होगी।
    Pessimistic = 130,

    // एक विश्वास स्तर सेट करें जो इस बात के प्रतिशत से मेल खाता है कि वास्तविक मान आशावादी और निराशावादी अनुमान के भीतर कितनी बार होंगे।
    // आप इसे मानक विचलन के मान के रूप में सोच सकते हैं: आपके अनुमान जितने अनिश्चित होंगे, रैंडम नंबर जेनरेटर में उपयोग किया गया मानक विचलन का मान उतना ही अधिक होगा
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// परियोजना जोखिमों का विश्लेषण करें
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// फ़ाइल पाथ द्वारा विश्लेषण को रिपोर्ट के रूप में फ़ाइल में सेव करें
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// या विश्लेषण को स्ट्रीम में सेव करें
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### संबंधित देखें

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


