---
title: "RiskAnalyzer.Settings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RiskAnalyzer प्रॉपर्टी। जोखिम विश्लेषण के लिए आवश्यक सेटिंग्स को परिभाषित करने वाले RiskAnalysisSettings क्लास का इंस्टेंस प्राप्त करता है या सेट करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks.riskanalysis/riskanalyzer/settings/
---
## RiskAnalyzer.Settings property

[`RiskAnalysisSettings`](../../riskanalysissettings/) क्लास का इंस्टेंस प्राप्त करता है या सेट करता है जो जोखिम विश्लेषण के लिए आवश्यक सेटिंग्स को परिभाषित करता है।

```csharp
public RiskAnalysisSettings Settings { get; set; }
```

## उदाहरण

रिस्क विश्लेषण को शुरू करने का तरीका दिखाता है, जिसमें &lt;see cref="Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings" /&gt; का उपयोग किया जाता है।

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
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

settings = new RiskAnalysisSettings
{
    IterationsCount = 300
};

// सेटिंग्स बदलें
analyzer.Settings = settings;

analysisResult = analyzer.Analyze(project);
earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### संबंधित देखें

* class [RiskAnalysisSettings](../../riskanalysissettings/)
* class [RiskAnalyzer](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalyzer/)
* assembly [Aspose.Tasks](../../../)


