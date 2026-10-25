---
title: "क्लास RiskPattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RiskAnalysis.RiskPattern क्लास। यह प्रोजेक्ट कार्य के लिए एक जोखिम पैटर्न का प्रतिनिधित्व करता है।"
type: docs
weight: 1930
url: /hi/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

प्रोजेक्ट कार्य के लिए जोखिम पैटर्न को दर्शाता है।

```csharp
public class RiskPattern
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | `RiskPattern` क्लास का नया उदाहरण आरंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | वास्तविक उत्पन्न मानों के आशावादी और निराशावादी अनुमान के भीतर रहने के प्रतिशत समय के अनुरूप विश्वास स्तर प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान CL99 है। |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | Monte Carlo सिमुलेशन में उपयोग किए जाने वाले प्रायिकता वितरण को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान ProbabilityDistributionType.Normal है। |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | सबसे संभावित कार्य अवधि का वह प्रतिशत प्राप्त करता है या सेट करता है जो सर्वश्रेष्ठ प्रोजेक्ट परिदृश्य में हो सकता है। डिफ़ॉल्ट मान 75 है, जिसका अर्थ है कि यदि अनुमानित कार्य अवधि 4 दिन है तो आशावादी अवधि 3 दिन होगी। |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | सबसे संभावित कार्य अवधि का वह प्रतिशत प्राप्त करता है या सेट करता है जो सबसे खराब प्रोजेक्ट परिदृश्य में हो सकता है। डिफ़ॉल्ट मान 125 है, जिसका अर्थ है कि यदि अनुमानित कार्य अवधि 4 दिन है तो निराशावादी अवधि 5 दिन होगी। |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | एक प्रोजेक्ट कार्य प्राप्त करता है जिस पर यह जोखिम पैटर्न लागू किया गया है। |

## उदाहरण

जोखिम सिमुलेशन सेटिंग्स को परिभाषित करने का तरीका दर्शाता है।

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// एक जोखिम पैटर्न प्रारंभ करें
var pattern = new RiskPattern(task);

// रैंडम नंबर जेनरेटर के लिए एक वितरण प्रकार चुनें जिससे संभावित मान उत्पन्न हों (वर्तमान में केवल दो प्रकार समर्थित हैं, अर्थात सामान्य और समान)।
// अधिक विवरण के लिए यहाँ देखें: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// सबसे संभावित कार्य अवधि का प्रतिशत सेट करें जो सर्वोत्तम प्रोजेक्ट परिदृश्य में हो सकता है
// डिफ़ॉल्ट मान 75 है, जिसका अर्थ है कि यदि अनुमानित कार्य अवधि 4 दिन है तो आशावादी अवधि 3 दिन होगी
pattern.Optimistic = 70;

// सबसे संभावित कार्य अवधि का प्रतिशत सेट करें जो सबसे खराब प्रोजेक्ट परिदृश्य में हो सकता है
// डिफ़ॉल्ट मान 125 है, जिसका अर्थ है कि यदि अनुमानित कार्य अवधि 4 दिन है तो निराशावादी अवधि 5 दिन होगी।
pattern.Pessimistic = 130;

// एक विश्वास स्तर सेट करें जो इस बात के प्रतिशत से मेल खाता है कि वास्तविक मान आशावादी और निराशावादी अनुमान के भीतर कितनी बार होंगे।
// आप इसे मानक विचलन के मान के रूप में सोच सकते हैं: आपके अनुमान जितने अनिश्चित होंगे, रैंडम नंबर जेनरेटर में उपयोग किया गया मानक विचलन का मान उतना ही अधिक होगा
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

settings.Patterns.Add(pattern);

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

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### संबंधित देखें

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


