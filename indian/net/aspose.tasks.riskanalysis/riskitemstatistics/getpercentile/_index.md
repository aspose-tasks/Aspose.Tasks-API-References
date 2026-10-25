---
title: "RiskItemStatistics.GetPercentile"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RiskItemStatistics मेथड। उत्पन्न नमूनों में से निर्दिष्ट प्रतिशत से कम मान प्राप्त करता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks.riskanalysis/riskitemstatistics/getpercentile/
---
## RiskItemStatistics.GetPercentile method

एक मान प्राप्त करता है जिसके नीचे उत्पन्न नमूनों का निर्दिष्ट प्रतिशत गिरता है।

```csharp
public DateTime GetPercentile(int percent)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रतिशत | Int32 | 0 और 100 के बीच निर्दिष्ट प्रतिशत। |

### रिटर्न वैल्यू

एक मान जिसके नीचे उत्पन्न नमूनों में से निर्दिष्ट प्रतिशत गिरते हैं।

## उदाहरण

जोखिमों के आँकड़े कैसे गणना करें, यह दर्शाता है।

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
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### संबंधित देखें

* class [RiskItemStatistics](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskitemstatistics/)
* assembly [Aspose.Tasks](../../../)


