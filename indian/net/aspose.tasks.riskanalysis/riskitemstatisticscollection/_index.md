---
title: "क्लास RiskItemStatisticsCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RiskAnalysis.RiskItemStatisticsCollection क्लास। RiskItemStatistics क्लास की इंस्टेंसेज़ को शामिल करने वाला संग्रह दर्शाता है"
type: docs
weight: 1910
url: /hi/net/aspose.tasks.riskanalysis/riskitemstatisticscollection/
---
## RiskItemStatisticsCollection class

[`RiskItemStatistics`](../riskitemstatistics/) क्लास की इंस्टेंसेज़ को शामिल करने वाला संग्रह दर्शाता है।

```csharp
public class RiskItemStatisticsCollection : IDictionary<Task, RiskItemStatistics>, 
    IEnumerable<RiskItemStatistics>
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Get](../../aspose.tasks.riskanalysis/riskitemstatisticscollection/get/)(Task) | इस संग्रह में निर्दिष्ट Task ऑब्जेक्ट से संबंधित [`RiskItemStatistics`](../riskitemstatistics/) क्लास की एक इंस्टेंस लौटाता है; यदि आइटम नहीं मिला तो null लौटाता है। |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskitemstatisticscollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |

## उदाहरण

जोखिम सांख्यिकी के संग्रह के साथ काम करने का तरीका दिखाता है।

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

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// सभी सांख्यिकीय आइटमों पर इटरेट करें
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish);

foreach (var statistic in statistics)
{
    Console.WriteLine("Short statistic: " + statistic);
    Console.WriteLine();
    Console.WriteLine("Statistic details: ");
    Console.WriteLine("Item Type: {0}", statistic.ItemType);
    Console.WriteLine("Expected value: {0}", statistic.ExpectedValue);
    Console.WriteLine("StandardDeviation: {0}", statistic.StandardDeviation);
    Console.WriteLine("10% Percentile: {0}", statistic.GetPercentile(10));
    Console.WriteLine("50% Percentile: {0}", statistic.GetPercentile(50));
    Console.WriteLine("90% Percentile: {0}", statistic.GetPercentile(90));
    Console.WriteLine("Minimum: {0}", statistic.Minimum);
    Console.WriteLine("Maximum: {0}", statistic.Maximum);
}

// या एक विशिष्ट सांख्यिकी प्राप्त करें
var itemStatistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Print the specific statistic: ");
Console.WriteLine("Expected value: {0}", itemStatistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", itemStatistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", itemStatistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", itemStatistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", itemStatistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", itemStatistics.Minimum);
Console.WriteLine("Maximum: {0}", itemStatistics.Maximum);
```

### संबंधित देखें

* class [Task](../../aspose.tasks/task/)
* class [RiskItemStatistics](../riskitemstatistics/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


