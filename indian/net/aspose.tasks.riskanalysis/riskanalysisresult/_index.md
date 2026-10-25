---
title: "क्लास RiskAnalysisResult"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalysisResult क्लास। जोखिम विश्लेषण का परिणाम दर्शाता है"
type: docs
weight: 1870
url: /hi/net/aspose.tasks.riskanalysis/riskanalysisresult/
---
## RiskAnalysisResult class

जोखिम विश्लेषण का परिणाम दर्शाता है।

```csharp
public class RiskAnalysisResult
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetRiskItems](../../aspose.tasks.riskanalysis/riskanalysisresult/getriskitems/)(RiskItemType) | निर्दिष्ट जोखिम प्रकार के लिए [`RiskItemStatisticsCollection`](../riskitemstatisticscollection/) का एक इंस्टेंस रिटर्न करता है। |
| [SaveReport](../../aspose.tasks.riskanalysis/riskanalysisresult/savereport/#savereport)(Stream) | जोखिम विश्लेषण रिपोर्ट को PDF फ़ॉर्मेट में स्ट्रीम पर सेव करता है। |
| [SaveReport](../../aspose.tasks.riskanalysis/riskanalysisresult/savereport/#savereport_1)(string) | जोखिम विश्लेषण रिपोर्ट को PDF फ़ॉर्मेट में निर्दिष्ट फ़ाइल पाथ पर सेव करता है। |

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


