---
title: "क्लास RiskPatternCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.RiskAnalysis.RiskPatternCollection क्लास. RiskPattern क्लास की इंस्टेंसेज़ को शामिल करने वाला संग्रह दर्शाता है"
type: docs
weight: 1940
url: /hi/net/aspose.tasks.riskanalysis/riskpatterncollection/
---
## RiskPatternCollection class

[`RiskPattern`](../riskpattern/) क्लास की इंस्टेंसेज़ को शामिल करने वाला संग्रह दर्शाता है।

```csharp
public class RiskPatternCollection : ICollection<RiskPattern>, IDictionary<Task, RiskPattern>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks.riskanalysis/riskpatterncollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |
| [Item](../../aspose.tasks.riskanalysis/riskpatterncollection/item/) { get; } | निर्दिष्ट कार्य के लिए [`RiskPattern`](../riskpattern/) क्लास की इंस्टेंस प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks.riskanalysis/riskpatterncollection/add/)(RiskPattern) | इस संग्रह में [`RiskPattern`](../riskpattern/) क्लास की एक इंस्टेंस जोड़ता है। |
| [Clear](../../aspose.tasks.riskanalysis/riskpatterncollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks.riskanalysis/riskpatterncollection/contains/)(RiskPattern) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks.riskanalysis/riskpatterncollection/copyto/)(RiskPattern[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskpatterncollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks.riskanalysis/riskpatterncollection/remove/)(RiskPattern) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |

## उदाहरण

रिस्क पैटर्न संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var settings = new RiskAnalysisSettings
{
    // मॉन्टे कार्लो सिमुलेशन के लिए इटरेशन की संख्या सेट करें (डिफ़ॉल्ट मान 100 है)।
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// जब तक RiskPatternCollection केवल-पढ़ने योग्य नहीं है
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// नए पैटर्न जोड़ सकते हैं
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// जोड़े गए पैटर्न पर इटरेट करें
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// इंडेक्स एक्सेस का उपयोग करके संग्रह में पैटर्न को संपादित करें
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// संपादन के बाद पैटर्न जांचें
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// हम पैटर्न को हटा सकते हैं
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// जाँचें कि पैटर्न संग्रह में नहीं है
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// संग्रह को दो तरीकों से साफ़ किया जा सकता है

// पैटर्न को एरे में कॉपी करें और एक-एक करके हटाएँ
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// या कोई पूरी तरह से पैटर्न संग्रह को साफ़ कर सकता है
settings.Patterns.Clear();
```

### संबंधित देखें

* class [RiskPattern](../riskpattern/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


